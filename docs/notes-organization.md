# How we organize notes

The root `index.html` links directly to each class's session index. Classes live in `semesters/<two-digit semester>/<class name>/`. Each class has an `index.html` listing session dates and weekdays, with links to its notes.

## Add a session

1. Start with finished NotebookLM HTML. If you have a Markdown summary, use it as source material in NotebookLM. Save the supplied HTML in the class folder as `YYYY-MM-DD.html`, using the session date. Confirm the date if it is missing.
2. Apply the shared page layout. Copy the masthead and contents markup from the [Requirement Engineering example](../semesters/01/Requirement%20Engineering/2026-11-19.html) and link [the shared stylesheet](../semesters/session-note.css) as `../../session-note.css`. Use `lang="fa" dir="rtl"`, a class name, a relative `index.html` return link, and a Persian weekday and date inside `<time datetime="YYYY-MM-DD">`. Put one sticky, horizontally scrolling contents bar above the lecture title. Give it short labels numbered with Persian digits and link each one to an existing section ID. Keep the lecture inside a `<main>` landmark.
3. Preserve the lecture content and useful interactions. Keep diagrams and tables readable on narrow screens by letting wide content scroll within its own container or by stacking its parts. Give diagrams a short text explanation and show chart values in text if a chart depends on an external library. Keep quizzes optional and omit progress tracking.
4. Add the session date, weekday, and relative HTML link to the class's `index.html`. Update the session count. When adding a new class, point its root index link directly to the class's `index.html` so it works when opened from disk.
5. Open the class index and follow the new link. Check the return link, section jumps, and diagram readability at a narrow viewport.

Use the [Warm Paper style guide](../editorial-warm-paper-style-guide.md) for visual details.
