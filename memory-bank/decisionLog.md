# Decision Log

This file records architectural and implementation decisions using a list format.
2025-03-05 21:29:55 - Log of updates made.

*

## Decision

*   [2025-03-05 21:29:55] Use an `<iframe>` to display chapter content (`Ch1.html`, `Ch2.html`) within `index.html`.

## Rationale

*   Simpler implementation compared to fetching and injecting content dynamically for this specific task.
*   Keeps chapter content separate and easy to manage.

## Implementation Details

*   The `index.html` will contain an `<iframe>` element.
*   Navigation links will target the `<iframe>` using its `name` attribute or JavaScript will update the `iframe.src` attribute.