# Using and running

## Visitor journeys

A visitor looking for background should use the About navigation link and read the agent introduction. A visitor looking for proof of work should use the Work section, inspect a slide's image and summary, and follow its source link if desired. A visitor ready to talk should use the contact area and choose email or the scheduling destination.

The carousel is editorial: it shows selected examples rather than an inventory search. Its next and previous controls loop continuously through the array. The dots allow direct selection. The visible caption and outgoing link should change with the image. If only the image changes or the source link points to a different example, stop treating the page as correct until the corresponding fields are reconciled.

An external scheduling page may ask for information or show availability. That experience belongs to the external service. The local site cannot promise an appointment exists until that service confirms it. Similarly, clicking email opens a composition action; the visitor must still send the message.

## Maintainer run and close

Start the Python preview in a dedicated terminal and keep its URL visible. Reload after source changes; there is no hot-reload service. If styles appear unchanged, verify you edited the served checkout and inspect the response before clearing all browser state.

Close the tab and stop the preview with Ctrl+C in its owning terminal. There is no database flush, queue drain, worker shutdown, or file upload in progress. Do not stop other projects' servers by killing every Python process or every listener on a guessed port.

## Backups and restore

The source repository and its static image assets are the complete local site artifact. Keep approved images in source control when their size is reasonable and usage rights are clear. Do not substitute private client documents or unapproved imagery into a public asset directory. A preview server exposes files under its root, so keep credentials and unpublished customer records outside that tree.

To recover from a broken change, use Git history to identify the last reviewed content and restore the affected file through a new scoped change. Preserve newer unrelated work. Recheck all relative asset paths and slideshow entries after the restore. There is no runtime database to restore, and rolling back the site does not cancel appointments held by an external service.
