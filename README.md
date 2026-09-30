# Gig Income Tracker

A free, private, single-page web app for delivery drivers (DoorDash, Walmart Spark,
Uber Eats, Amazon Flex, Roadie, Instawork) to log every shift and see their **real**
earnings: dollars per hour, dollars per mile, and net after expenses.

No account. No server. No tracking. Your data stays in your browser's localStorage —
nothing ever leaves your device.

## Features

- Log shifts: date, platform, hours, base pay, tips, miles, gas/other expenses
- Live dashboard: total earned, net after expenses, $/hour, $/mile, hours, miles
- Per-platform breakdown table (which app actually pays you best?)
- Shift history with one-tap delete
- Export everything to CSV for taxes or bookkeeping
- Mobile-friendly dark UI — works great as a phone home-screen app
- Form validation (no zero-hour or negative-dollar entries)

## How to use

1. Open `index.html` in any browser (double-click it, or serve it — no build step).
2. Fill in the shift form and hit **Add shift**.
3. Watch your $/hour and $/mile update live.
4. Use **Export CSV** at tax time.

To install on your phone: open the page in your mobile browser → Share → Add to Home Screen.

## Tech

- Single HTML file, zero dependencies, zero network calls
- Vanilla JS + localStorage (`gigIncomeTracker.v1`)
- Pure logic functions (`validateShift`, `calcStats`, `toCSV`) are DOM-free and unit-tested

## Privacy

All data is stored only in your browser via localStorage. There is no backend, no
analytics, no cookies, and no data transmission of any kind.

## License

MIT — see [LICENSE](LICENSE).
