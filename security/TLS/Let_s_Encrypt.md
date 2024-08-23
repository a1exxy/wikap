# Ограничения LE
Источник: https://letsencrypt.org/docs/staging-environment

Rate Limits

The staging environment uses the same rate limits as described for the production environment (https://letsencrypt.org/docs/rate-limits/) with the following exceptions:

- The Certificates per Registered Domain limit is 30,000 per week.
- The Duplicate Certificate limit is 30,000 per week.
- The Failed Validations limit is 60 per hour.
- The Accounts per IP Address limit is 50 accounts per 3 hour period per IP.
- For ACME v2, the New Orders limit is 1,500 new orders per 3 hour period per account.