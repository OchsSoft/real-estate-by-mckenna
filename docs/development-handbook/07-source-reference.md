# Source reference

This edition follows `OchsSoft/real-estate-by-mckenna` at committed revision `3f38e3528bd1c679f50ae23f34a0b87050623e5b`. Line links below point to that exact revision, so later changes cannot silently change the meaning of a reference. The handbook explains source behavior and identified gaps; it is not a claim that a new installation or production workflow was exercised.

## Read the implementation

- [index.html at line 11](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L11): Inline visual system and responsive rules.
- [index.html at line 660](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L660): Portfolio section and carousel DOM contract.
- [index.html at line 754](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L754): Authored slide record schema and public content.
- [index.html at line 823](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L823): Accessible dot creation and focus-replacement boundary.
- [index.html at line 839](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L839): Wrapped index and synchronized image/caption/link update.
- [index.html at line 850](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/index.html#L850): 6500 millisecond interval and reduced-motion guard.
- [README.md at line 1](https://github.com/OchsSoft/real-estate-by-mckenna/blob/3f38e3528bd1c679f50ae23f34a0b87050623e5b/README.md#L1): Minimal repository entry point and existing quick guide.

## Verify the edition

Before following a development recipe, compare the current checkout with this revision. Read `git status --short` to identify existing edits and `git log -1 --oneline` to identify the current commit. A newer primary branch may intentionally change commands, schemas, or routes. Reconcile those changes in the corresponding chapter before relying on an old instruction. Preserve the quick operations guide as the shorter entry point.

Source inspection does not establish end-to-end acceptance. Test names and commands describe evidence that a maintainer can obtain. Keep actual execution results beside the review for the change being made, and distinguish a skipped or blocked test from a passing one. Runtime data, credentials, build directories, and generated test output do not belong in source control.
