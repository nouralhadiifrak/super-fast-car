# Super Fast Car

Car rental website for Super Fast Car, Casablanca. One static page (French by default, with English and Arabic), deployed on Vercel.

- `index.html`: the whole site. Phone/WhatsApp, Instagram and the map link are in `CONFIG` near the top of the script.
- `images/cars/`: fleet photos. `images/hero-car.webp`: hero photo.

Images are cached by browsers for 30 days (`vercel.json`). When you replace a photo, give the new file a new name (e.g. `hero-car-v4.webp`) and update `index.html`; otherwise visitors keep seeing the old one.

## Owner dashboard (demo)

`/dashboard` is a demo management space for the owner (French): today's departures and returns, pending requests, alerts (late returns, insurance, technical inspection, oil change, vignette, unpaid balances), a day-by-day planning of every car, bookings (create, confirm, departure, return, extend, payments, printable contract), fleet and maintenance, clients (history, blacklist) and finances (revenue, expenses, profit).

It has no server: data is example data stored in the visitor's browser (`localStorage`), resettable from Paramètres. A booking sent from the site's form in the same browser appears in the dashboard as "En attente". A real version would need a database and a login.
