# Review insights dashboard

A simple dashboard that shows guest review insights for four hotel properties.

## What it shows
- Average rating, review count and share of low ratings
- Average rating by month
- Complaints by theme (cleanliness, noise, staff, security, location)
- Latest low-rated reviews that need attention
- A one-line summary that updates with the property filter

## Run it
No install needed. Open `index.html` in a browser, or use the Live Server extension in VS Code.

## Deploy
Push this folder to GitHub, then import the repo in Vercel or Netlify. No build step is needed.

## Data
The reviews are generated sample data (a fixed seed, so results stay the same). I did not scrape Booking.com, because that breaks its terms. To use real data, replace the `data` array in `index.html` with an export of real reviews, using the same fields: property, month, rating, theme, text, date.

## Choices and trade-offs
- Plain HTML, CSS and JavaScript: fast to load, nothing to install, easy to review.
- Bars are drawn with CSS instead of a chart library to keep the page small.
- With more time I would add a date-range filter, a backend, and an AI-written reply to negative reviews.
