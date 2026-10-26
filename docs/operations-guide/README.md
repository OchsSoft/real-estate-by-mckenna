# Real Estate by McKenna Operations Guide

This repository is an independent static website. A local preview serves HTML, styles, JavaScript, and images. It does not run a customer database, send a message, process an order, or alter the deployed website.

## Start the local preview

The tree contains index.html and local images, but no launch script. The command below is a proposed loopback-only preview to verify locally. Use a native Python environment and run from this repository root:

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

Open http://127.0.0.1:4173. If another process owns that port, inspect it and choose an unused preview port rather than stopping another project. No npm installation is required for the inspected static tree.

## Check that it works

Inspect the first page, images, navigation, mobile width, and the particular content you changed. Inspect the intended links and content without submitting production requests. A good preview does not prove external delivery, booking, payment, DNS, or production hosting.

## Troubleshoot

A directory listing usually means the chosen folder does not contain index.html. Missing images can be relative-path or capitalization errors; Linux paths are case-sensitive. Keep an external-service failure separate from a static-page problem. Confirm the exact repository before editing.

## Close and maintain

Save source changes and any publishable review output. Press Ctrl+C in this preview's terminal and wait for the prompt. Closing the browser alone does not stop the server. A local stop does not take down the published website. Review changes in an independent master-targeted topic PR; deployment remains separate and human-controlled.

## Before you begin

Use this repository root or the precise client/server folder named above. If an installed supervisor already owns this instance, use it instead of starting a second copy. A process is one running program; a port is its numbered network doorway. The address 127.0.0.1 means this machine only.

## Keep troubleshooting scoped

Record the first error, source revision, working directory, and selected instance. Check the stated prerequisites before changing anything. Preserve useful work before resets. Stop only the process or dedicated dependency you own; do not kill by a guessed port or broad name. Keep credentials and private records out of reports. Migrations, seeds, volume deletion, deployment, and new model downloads are separate operations, not generic restart fixes.

## Normal operating sequence

![Normal operating sequence](operating-flow.svg)

## Maintaining this guide

Keep this Markdown, the editable Word edition, PDF, and operating-flow.svg together here. Update them when merged commands, storage, dependencies, or limits change. Edit Word and export PDF independently when convenient, then inspect the affected pages. No running AIOS service is needed to read or maintain these documents.

Source-defined instructions and known gaps are distinguished above. This documentation task did not launch the application or prove a new production workflow. Verify changes locally on NixOS; use a topic PR and human merge for owned source. Deployment is separate, and routine hosted CI remains disabled.

## Source and edition

Edition 26 October 2026. Repository OchsSoft/real-estate-by-mckenna. Inspected source revision `6966d295ff041672808df539b65788b3cd15a945`.

Source files: [index.html](https://github.com/OchsSoft/real-estate-by-mckenna/blob/6966d295ff041672808df539b65788b3cd15a945/index.html).

[Editable Word edition](Operations_Guide.docx) | [PDF edition](Operations_Guide.pdf)
