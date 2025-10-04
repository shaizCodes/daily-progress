# Day 003 Progress Log

This README summarizes the work done on Day 003, following the daily log convention defined in the root README.

**DATE:** _Thursday, August 07, 2025_

**Attendance:** _06:01 PM to 03:26 AM (**Birthday**)_

## Tasks/Activities
- Created a repository to document daily progress at [CoderzHunt](https://coderzhunt.com/)
- Investigated approaches to bypass [Cloudflare](https://www.cloudflare.com/en-gb/) on npidb.org; experimented with [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/index.html) (Python) and [Puppeteer](https://pptr.dev/) (Node)
- Signed up on [Cursor](https://cursor.com/agents) with official email and used it to scaffold a Node-based NPI DB scraper
- Joined the official [WhatsApp](https://www.whatsapp.com/) group and introduced myself
- Installed [Postman](https://www.postman.com/) and tested initial API endpoints for the Node scraper
- Created a Puppeteer-based sample solution that bypassed the verification challenge and scraped HTML table data

## Tools/Technologies
- GitHub
- Cursor
- Node.js
- Python
- Postman
- PyAutoGUI
- Puppeteer
- Selenium

## Blockers
- [x] Cloudflare anti-bot protection caused repeated re-verification when using Selenium
- [x] PyAutoGUI is not suitable for structured scraping via the DOM; it would require screenshots and OCR, which is error-prone
- [x] Interim workaround: switched to Puppeteer (Node) and built a few API endpoints to support the upcoming Chrome extension

## Details
- PyAutoGUI can control real browser windows, but reliable data extraction would require screenshots + OCR with potential accuracy issues
- Selenium keyboard-event attempts still triggered Cloudflare re-verification loops in automated/testing environments
- Cursor AI assisted in scaffolding Node API endpoints for the npidb.org scraper
- Personal: Birthday celebrated, played Tekken on PS5

