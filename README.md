# Corgi Fun Money

A cute React budgeting app for a $1,000 monthly fun-money budget.

## Included

- Month-by-month spending
- Corgi and heart theme
- Category pie chart
- 12-month trend
- Spending history and CSV export
- Savings goals
- Wishlist
- Achievement cards
- Local browser storage
- Firebase setup file for optional future cloud sync

## Run locally

1. Install Node.js.
2. Open a terminal in this folder.
3. Run:

```bash
npm install
npm run dev
```

## Deploy with Vercel

1. Upload this folder to a GitHub repository.
2. Sign in to Vercel.
3. Choose **Add New → Project**.
4. Import the GitHub repository.
5. Vercel should detect Vite automatically.
6. Click **Deploy**.
7. Copy the public Vercel URL.
8. In Notion, type `/embed` and paste the URL.

## Firebase cloud sync

The app works immediately using local browser storage. Firebase credentials are not included.

To prepare Firebase:

1. Create a Firebase project.
2. Enable Authentication and Firestore.
3. Copy `.env.example` to `.env`.
4. Fill in the Firebase web app values.
5. Add authentication and Firestore security rules before storing real financial data.

The included `src/firebase.js` initializes Firebase when those values are present, but full sign-in and syncing still need to be wired to your preferred authentication flow.
