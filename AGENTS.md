# Trials

Each trial tests one tool, or compares several, against one question and ends
with a one-page verdict. This repository is public: use synthetic or public
inputs, and keep anything from real documents or accounts in the trial's
ignored `private/` folder.

## Start

1. Copy `template/` to `YYYY-MM-<tool>/`, or `YYYY-MM-<tool>-vs-<tool>/` for a comparison.
2. Fill in `BRIEF.md` before running anything.
3. Add a row to the index in `README.md` with the verdict `running`.

## Run

- Write each case as one file in `cases/`: the input, the steps, and what a good
  result looks like. Start from the cases in [edge-cases.md](edge-cases.md) that
  apply, then add cases specific to the tool.
- Save raw output in `runs/<case>/<tool>.md` (or the format the tool produces),
  unedited, with the date and tool version at the top.
- When a case needs real documents or accounts, keep its inputs and outputs in
  `private/` and commit only a description of the case and the result.

## Finish

1. Write `ONE-PAGER.md` in the template's format. Link every claim to a case or run.
2. Replace `running` in the index with the one-pager's first line and the date.
3. Commit and push.

Trials listed in `.gitignore` predate this repository and keep their own
repositories and rules; follow the `AGENTS.md` inside each one.
