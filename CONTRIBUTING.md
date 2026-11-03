# Contributing

This repository tracks weekly Apple (AAPL) option expiration data for the risk meeting.

## Process

1. Pull the current market data from Yahoo Finance (price, expiration dates, chains).
2. Create or update the tracking issue per expiration, titled `Expiry YYYY-MM-DD`.
3. Update the per-expiration stats and the per-expiration summary table.
4. Open a pull request from the feature branch (`add-expirations-doc`) into `main`.
5. After review, merge and keep `main` current with the default branch.

## Data quality

- Share price for at-the-money computation is taken from the live source on the day of pull.
- Where the source returns an empty ZZ index or an odd value, report exactly what the source returned.
- Every cost of symbols used in our四人ين report...
