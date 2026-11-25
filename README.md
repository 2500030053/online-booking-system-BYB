# BYB – Book Your Buzz (React)

A student-friendly event ticket booking website built with **React, Vite, CSS and Local Storage**.

## Run the project
1. Extract this ZIP file.
2. Open the extracted **BYB_React_New** folder in VS Code (the folder that contains `package.json`).
3. Open Terminal in that folder.
4. Run these commands one by one:

```bash
npm install
npm run dev
```

5. Open the **Local** URL shown in the terminal (usually `http://localhost:5173/` or `http://localhost:5174/`). Keep the terminal running.

## Demo login
- User: `demo@byb.com` / `1234`
- Admin: `admin@byb.com` / `admin123`

## Modules
- `src/modules/AuthModal.jsx` – Login and registration
- `src/modules/EventCard.jsx` – Event card UI
- `src/modules/BookingModal.jsx` – Ticket quantity, ticket type and booking confirmation
- `src/modules/Tickets.jsx` – User's booked tickets
- `src/modules/DashboardModal.jsx` – User and admin dashboards
- `src/data/events.js` – Sample event data
- `src/utils/storage.js` – Local Storage functions
- `src/App.jsx` – Main app and module connections

## Features
- Search and filter events by category
- Register, login and logout
- Book 1–8 tickets and choose Standard or Premium
- Store bookings and user accounts in Local Storage
- View personal tickets and user dashboard
- Admin dashboard with bookings, users, tickets and demo revenue

## Important
This is a frontend college demo. No real payment is processed and data stays in the browser's Local Storage. To reset demo data, clear Local Storage for the local website in your browser.


## Registration and login flow
1. Create an account with name, email and password.
2. BYB saves the new account in this browser's Local Storage (`byb_users`).
3. The app displays an account-created message and switches to the Login tab.
4. The user must enter the same email and password to log in.

## Where are registered accounts stored?
- `src/App.jsx`: the `register` function creates the account and adds it to the users list.
- `src/utils/storage.js`: `getUsers()` reads accounts from Local Storage and `saveUsers()` saves them under the key `byb_users`.
- `src/modules/AuthModal.jsx`: contains the Create Account and Login forms.

This is a frontend student-project demo. Accounts are stored in the browser that created them; they are not stored on a shared server or automatically available on another computer/browser.
