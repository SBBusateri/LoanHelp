# LoanHelp

A tiny static site that demonstrates the avalanche payoff math for a few mocked student loans.

## How to run locally

Open `index.html` in your browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## How to push to GitHub

```bash
git init
git remote add origin https://github.com/SBBusateri/LoanHelp.git
git add .
git commit -m "Initial LoanHelp avalanche calculator"
git branch -M main
git push -u origin main
```

## How to deploy to Vercel

Install the Vercel CLI if you haven't:

```bash
npm i -g vercel
```

From this project directory, run:

```bash
vercel
```

Vercel will detect the static `index.html` and deploy it.

## Notes

- Assumes monthly compounding at the effective annual interest rate.
- Enter an extra monthly payment in the UI to see each loan's payoff months, total interest, and total paid under an avalanche plan (extra cash goes to the highest-rate loan first).
- The mock loans are based on the first DIRECT SUB loan data provided.
