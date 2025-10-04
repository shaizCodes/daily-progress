# Day 015 Progress Log

This README summarizes the work done on Day 015, following the daily log convention defined in the root README.

**DATE:** _Monday, August 25, 2025_

**Attendance:** _06:09 PM to 04:30 AM_

## Tasks/Activities

- guided intern in setting up a MongoDB connected ExpressJS backend with basic CRUD operations
- demonstrated and assigned him tasks related to Gemini CLI for code assistance, and Postman for API testing
- explained the project structure and workflow of Jobalize
- completed the task: resolved OTP input failure

## Tools/Technologies

- JavaScript, ExpressJS, and NodeJS
- Gemini CLI
- Postman
- MongoDB (Atlas, and Community Edition/Server)

## Blockers

- The submit button remained disabled despite having filled all required fields. [RESOLVED]

## Details

- I used Gemini CLI to write the `fillOTP(page, OTP)` function by providing it the HTML snippet of the OTP section, which was successful in filling the OTP section, however, I encountered the disabled submit button despite completely filling the form. I inspected the button and OTP input fields, and manipulated the DOM to enable the submit button. I toggled the target attributes (i.e., `disabled`, `aria-disabled`) and class names (i.e., `btn__disabled`), but it did not work. I manually removed the target attributes and classes, but it did not work. I tried faking human interaction by focusing the input then typing in the OTP, and triggering multiple events (i.e., `input`, `change`, `blur`, `focus`), but it did not work. I was about to try other possibilities, but, Software Engineer Abdul Manan managed to resolve that using Cursor.
