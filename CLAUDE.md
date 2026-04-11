# Project notes

## Which files to edit

Only the Windows 11 flow is in scope. The editable files are:

- `Win11.psm1` — functions module
- `Win11.ps1` — entry point
- `mh-win11.preset` — preset selecting which functions run
- `mh-win11-run.bat` — runner
- `Regfiles/` — .reg files consumed by `BunchOfTweaks` and related functions

Do NOT edit anything else in this repo (the Win10 scripts, the `Default.*` files, or the `pulecny` variant listed below) unless explicitly asked.

## Files to leave alone

- **`Win11-pulecny.psm1`**, **`mh-win11-pulecny.preset`**, and **`mh-win11-run-pulecny.bat`** — these are a separate variant for another user ("pulecny") and must NOT be updated when changes are made to the main `Win11.psm1` / `mh-win11.preset` / `mh-win11-run.bat` flow. Even if `Win11-pulecny.psm1` contains a parallel `BunchOfTweaks` with overlapping logic, do not mirror changes into it.
