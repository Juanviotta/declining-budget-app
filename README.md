# declining-budget-app
Declining Budget App for Family Finances.

A single-page web app (`index.html`) for a shared monthly budget that counts down as spending is logged. Data syncs between phones through Firebase Firestore.

## Using it
- Open the page, pick your profile and enter your PIN. The app remembers the last profile on that phone.
- Tap **+** to log an expense. It starts on today's date and the last category you used.
- Home shows what's left this month and how much that allows per day for the rest of the month.
- Tap a category to see its expenses, log straight into it, or change its budget for this month only.
- Deleting an expense can be undone from the message that appears.

## Changing a PIN
PINs are stored as hashes in `index.html` (`PIN_HASHES`). Open the app, run `await hashPin("JVO", "1234")` in the browser console with the new PIN, and paste the result into `PIN_HASHES`.
