# Developing and testing

## Recipe: add or replace a work example

Prepare an approved web image under `assets/` with a descriptive stable filename. Optimize it before committing; an oversized photo affects every visitor. Add a `slides` entry containing all five fields. Write alternative text that describes the useful visual information rather than repeating “image of.” Keep status and narrative accurate for the example and confirm the source destination is intended for public visitors.

Load the preview, navigate directly to the new dot, and verify image, alternative text in the DOM, title, caption, and URL together. Test first-to-last and last-to-first wrapping after changing the array length. Wait for automatic rotation with normal motion settings and repeat with reduced motion. A missing array comma can prevent the entire script from parsing, so inspect the console.

## Recipe: change contact or positioning

Search `index.html` for all copies of the old text or destination. Visible contact wording, link URLs, headings, and metadata can diverge if only one occurrence changes. Update the intended fields together without altering unrelated property stories. Review external links for correct scheme and destination; `mailto:` is an email action, not an HTTPS page.

For a scheduling replacement, agree on the approved external endpoint first. The current implementation needs only a link change. Do not add a client-side API token or collect inquiries in an improvised browser store. If an embedded form becomes necessary, design success, failure, spam control, privacy, retention, and accessible errors as a separate feature.

## Recipe: separate the one-file implementation

If the inline style or script becomes difficult to maintain, extract it into dedicated assets without changing behavior in the same step. Move CSS to a stylesheet and the slideshow to a script that loads after its required elements. Keep relative asset resolution equivalent; JavaScript strings used as DOM image URLs resolve relative to the page, which is easy to confuse with module-relative paths.

Acceptance should compare the page before and after extraction: layout, all eight slides, keyboard controls, reduced motion, and contact links. A refactor is complete when the observable behavior is preserved, not merely when new files exist. Avoid adding a framework until there is a concrete product need that outweighs its install and build complexity.

## Recipe: improve carousel access

Introduce a visible pause/resume control and preserve the user's choice across manual navigation within the page. Consider listening for changes to reduced-motion preferences and pausing while the page is hidden. Maintain stable dot elements instead of recreating the focused element on every slide change.

Test with keyboard only: focus a dot, activate it, and confirm focus remains predictable. Pause, wait longer than 6500 milliseconds, and confirm the slide stays fixed. Resume, verify rotation, then enable reduced motion and confirm the stronger preference wins. These are proposed acceptance criteria; the existing baseline has no automated tests for them.

## Review and maintainability

Keep source files reasonably below the workspace's 1000-line threshold as features grow. This baseline's single file is already substantial, so extraction is a practical split plan before adding a larger gallery or lead interface. Preserve the site's simple static deployment and explain any new dependency or service in this handbook. A small site should stay understandable without reconstructing an undocumented toolchain.
