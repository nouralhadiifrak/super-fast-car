# Super Fast Car

Car rental website for Super Fast Car, Casablanca. One static page (French by default, with English and Arabic), deployed on Vercel.

- `index.html`: the whole site. Phone/WhatsApp, Instagram and the map link are in `CONFIG` near the top of the script.
- `images/cars/`: fleet photos. `images/hero-car.webp`: hero photo.

Images are cached by browsers for 30 days (`vercel.json`). When you replace a photo, give the new file a new name (e.g. `hero-car-v4.webp`) and update `index.html`; otherwise visitors keep seeing the old one.
