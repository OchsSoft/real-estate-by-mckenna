# Gaps and recovery

## Symptom diagnosis

| Symptom | Evidence to inspect | Safe action |
| --- | --- | --- |
| Page is a directory listing | Server root and requested URL. | Start preview from repository root. |
| Image is broken | Network 404, exact filename and case. | Repair the slide path or restore the approved asset. |
| Carousel never changes | Console parse error, missing DOM ID, reduced-motion preference. | Fix the specific script error; manual-only behavior under reduced motion is expected. |
| Caption and image disagree | The selected slide object and `setSlide`. | Correct the complete entry as one editorial change. |
| Focus disappears after dot activation | `renderDots` replaces the focused element. | Preserve stable controls in a scoped accessibility fix. |
| Email or scheduler did not complete | External application confirmation. | Explain the handoff and verify its destination; do not claim a saved local lead. |
| Live site differs from preview | Deployed revision and host cache. | Identify the released source before changing content again. |

## Prioritized gaps

**Accessible slideshow control:** `restartTimer` has a reduced-motion startup check but no explicit pause control and `renderDots` rebuilds controls. Add stable focus, pause/resume, and preference-change handling. Acceptance is a keyboard journey and a timed pause demonstration.

**Repeatable checks:** there is no automated test or pinned Nix environment. Add a small deterministic static/browser validation path, then demonstrate it on NixOS. Keep external scheduling and email submission outside routine tests.

**Maintainability of one file:** content, CSS, and behavior share `index.html`. Extract concerns before the file exceeds maintainable size; preserve all DOM contracts and compare the rendered page locally. Avoid mixing a mechanical split with a redesign.

**Release documentation:** no complete host/deployment contract is established in source. Document the actual host, artifact root, domain ownership, rollback process, cache behavior, and human release gate when verified. Do not infer these from a public domain alone.

**Content maintenance:** static success stories can become stale. Assign an editorial review cadence and require approval for changes in property status or claims. This is separate from a technical uptime check.

## Things to avoid during repair

Do not add a database because a contact link did not send email. Do not rewrite the site because one image path is wrong. Do not expose private customer or internal stack data to make a public page appear more complete. Work from the failing layer, use the smallest complete repair, and retain real preview evidence with the review.
