# Day 037 Progress Log

This README summarizes the work done on Day 037, following the daily log convention defined in the root README.

**DATE:** _Wednesday, September 24, 2025_

**Attendance:** _06:07 PM to 03:13 AM_

## Tasks/Activities

- Implemented a binary semaphore to ensure only a single Chrome instance is launched for concurrent requests.
- Developed a Windows batch script that allows users to choose a Chrome profile and open it in debug mode so Puppeteer can attach. I tried explaining this unnecessary thing last week but was ignored, so I came up with this solution, other than the Chrome extension one...
- Created symlinks for Chrome profiles selected by users running the batch script.
- Pushed the latest code to the drafted Pull Request for review.
- Completed assigned backend tasks.
- Integrated a PDF generation API; however, the provider uses a deprecated library (unmaintained since March 2018) and will require migration.

## TODOs / Pending

- Minor UI validation tasks pending.
- Possible follow-up tasks for tomorrow:
  - Migrate PDF generation service to use Puppeteer.
  - Test & upgrade form field extraction and filling.
  - Implement pause/lock and resumable backend workflow.

## Tools/Technologies

- Puppeteer / headless Chrome
- Windows batch scripting
- Symlink management
- Backend services and APIs

## Blockers

- PDF generation API depends on a deprecated library; migration required to a maintained solution.

## Details

- The binary semaphore design reduces the risk of multiple Chrome instances causing resource contention. The Windows batch script improves developer ergonomics by making it easy to attach Puppeteer to an existing profile in debug mode. The PDF generator migration is prioritized due to the deprecated dependency.
