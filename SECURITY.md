# Security policy

## Reporting a vulnerability

Email **macd@macd.ie** with the repository name, what you found and how to
reproduce it. Please do not open a public issue or discuss the finding
publicly until we have shipped a fix.

We aim to acknowledge reports within 3 working days and to give a first
assessment within 10. This is a small company; thank you for giving us the
time to fix things before disclosure.

## Scope

All repositories under `macd-adaptive-limited` and `macd-adaptive`, and the
services they deploy (macd.ie and its subdomains, booking and panel APIs).

Out of scope: findings that need access to a customer's account or data,
denial-of-service volume testing, and issues in third-party services we do
not operate.

## Practices

- No secrets in git; generated keys go straight to the owner-managed secret
  store. Secret scanning (gitleaks) runs in CI where configured.
- Money movement, email sending and other external effects live behind
  flags that are OFF by default and are activated only with the owner's
  explicit approval.
- Dependencies are reviewed through lockfiles and PR review.
