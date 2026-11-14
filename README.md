# UAE KYC Verify

A single-file web app for KYC (Know Your Customer) verification of UAE businesses: trade licence, FTA Tax Registration Number (TRN), Emirates ID, ultimate beneficial owners and AML screening, plus a reviewer queue with risk scoring.

## Run

Open `index.html` in any modern browser. No build step or server needed.

- **Apply tab:** 6-step applicant wizard with format checks for the TRN (15 digits, starting with 100), the Emirates ID (784 prefix, Luhn checksum, birth year matching the date of birth) and UAE mobile numbers, and expiry checks for the licence and Emirates ID.
- **Reviewer tab:** approve, reject or request info, with an audit history, risk score and factors, and CSV export. Use **Load sample data** for a demo.

## Limitations

- Data is stored in the browser's `localStorage` only, and uploaded files are not stored.
- The app checks TRN format but cannot confirm that a TRN is active. Use the FTA's official TRN verification on tax.gov.ae. Sanctions screening must be done against the official UAE and UN lists.
- This app is not affiliated with the UAE Federal Tax Authority or any government body.
