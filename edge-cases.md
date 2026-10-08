# Standard edge cases

A starting list; add cases here when a trial finds one worth repeating.

1. **Large input:** a document or dataset well past typical size (e.g. 100+ pages).
2. **Rich structure:** tables, nested lists, comments, suggestions, images, footnotes.
3. **Non-English text:** Spanish with accents, plus a right-to-left script.
4. **Expired or missing auth:** what the tool says, and whether it recovers.
5. **Partial failure:** interrupt a run halfway; check what was left behind.
6. **Concurrent edit:** someone else changes the target while the tool works.
7. **Round trip:** read, change nothing, write back; diff the result.
