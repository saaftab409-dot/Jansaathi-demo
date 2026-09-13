# JanSaathi — SIH 2026 civic grievance demo

A responsive, front-end prototype of a multi-modal civic-grievance experience. It is deliberately local-only: accounts, complaints, uploads and simulated workflow state are held in this browser's local storage.

## Run it

No installation or build step is required.

1. Open `index.html` in a modern browser, or start a static server in this folder:

   ```powershell
   python -m http.server 8080
   ```

2. Visit `http://localhost:8080`.
3. Choose **Register**, click **Get demo OTP**, and use `2026` to complete the simulated verification.
4. Create a complaint and follow it through routing, proof, escalation and rating.

## Included demo flows

- Responsive landing page and dashboard
- Local account registration, profile picture, generated Citizen ID, password login and lock/re-login
- A clear 3-way chooser: text complaint, local audio recording, or AI-style browser voice-to-text; voice-to-text complaints can download their local transcript as a `.txt` file
- Optional image/video/audio selection and browser geolocation request
- Simulated category/location routing to fictional PWD, Nagar Nigam, NHAI, Jal Kal and Junior Engineer records
- Department routing choice: let the AI demo suggest a department from category/location, or manually select PWD, Nagar Nigam, NHAI or Jal Kal
- Officer and citizen contact cards, SLA, escalation, timeline and status tracking
- Simulated before/after proof GPS validation and 5-star resolution rating

## Important demo boundaries

JanSaathi does **not** send OTPs, make calls, upload evidence, contact real officers, access any government routing service, or validate real GPS metadata. Names, contact details, routes and locations are fictional prototype data. Browser microphone, speech and location capabilities work only when the browser supports them and the user permits access.
