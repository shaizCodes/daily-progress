# Day 035 Progress Log

This README summarizes the work done on Day 035, following the daily log convention defined in the root README.

**DATE:** _Monday, September 22, 2025_

**Attendance:** _06:15 PM to 03:15 AM_

## Tasks/Activities

- Fixed an audit log bug by adapting to a new API endpoint requirement.
- Refactored the codebase to use a resource-efficient custom headless browser profile instead of copying profiles which caused buffer overflow issues.
- Implemented methods to retrieve unprocessed *** by profile id, connect Puppeteer, and launch Chrome efficiently.
- On process failures, preserved the tab and displayed an error toast in the top-right of the screen as requested.
- Removed unnecessary browser cleanup calls and reduced hundreds of lines of code by returning early to break flow where appropriate.
- Added TODO comments to guide the next refactor cycle.
- [TODO] Implement or utilize web workers to improve concurrency.
- [EXTRA] Before coming to office I had the laptop with me at hostel, I scanned and troubleshot laptop issues which were causing unexpected shutdowns. Realized it was a hardware issue likely due to RAM. Spent around 6 hours diagnosing and planning for repair. Fortunately, the shutdown issue became less frequent, allowing me to continue working.

## Tools/Technologies

- Puppeteer / headless Chrome
- JavaScript/Node.js
- Browser session and profile management
- API integrations

## Blockers

- No blockers reported; next steps are to implement concurrency improvements with web workers.

## Details

- The refactor reduced memory overhead and prevented buffer overflows by avoiding profile duplication. Error handling now preserves state for failed applications to allow manual intervention or retries. Further concurrency improvements are planned.
