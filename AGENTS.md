<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Calculation math lives in src/lib/calc.ts and grading tables in src/lib/grading.ts, separate from UI; keep src/lib/calc.test.ts updated when rules change.
- A grading scheme may be marked `verified: true` only when its grade points, course-inclusion rules and percentage formula were read from an official institution document, with that document's URL in `source` and the clause cited; third-party summaries are never grounds for verification. Keep src/lib/grading.test.ts asserting each verified scheme's exact table so a later edit cannot silently drift from the document.
