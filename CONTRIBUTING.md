# Contributing

This repository is the weekly AAPL (Apple Inc.) option expiration tracker, built to be re-run each week before the risk meeting.

## Weekly workflow

1. **Pull market data from Yahoo Finance:** current share price, option expiration dates, and the chain data for each tracked expiration.
2. **Create one tracking issue per expiration**, titled `Expiry YYYY-MM-DD` (the real date substituted). Each issue body must contain the share price used plus the at-the-money strike, the highest-open-interest call strike, and the highest-open-interest put strike.
3. **Document the per-expiration statistics** in the tracking file and in the per-expiration summary table.
4. **Open a pull request** from the feature branch (`add-expirations-doc`) into `main` once all issues for the cycle are created and the full expiration map is drafted.
5. **Keep the default branch current:** add further notes, doc fixes, or follow-up items, then update the feature branch from `main` before the final merge.

## Data-quality rules

- The share price used for the at-the-money computation is the one returned by the source on the day the data is pulled.
- Where the source returns an unusual or empty value, report exactly what the source returned rather than substituting another number.
- Contract data is quoted per listing as returned, including any odd volume or open-interest quirks in the source.

## Traceability

Issues in this repo track each weekly expiration cycle. The pull request that closes a cycle is the record used for the risk-meeting deck.
