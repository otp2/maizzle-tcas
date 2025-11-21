# Twin Cities Auto Show email kit

This kit adds three ready-to-edit Maizzle templates for the Twin Cities Auto Show and documents how to export them for Mailchimp.

## Brand palette
- Midnight blue: `#004391`
- Sky blue: `#91C5E6`
- Violet: `#3D2B75`
- Charcoal: `#262730`
- White: `#FFFFFF`

## Templates
- `emails/autoshow-save-the-date.html`: announcement with key dates, hours, and primary CTAs.
- `emails/autoshow-highlights.html`: programming overview covering exhibits, family activities, and test drives.
- `emails/autoshow-last-call.html`: final reminder with packing tips and arrival guidance.

Each template uses consistent typography, spacing, and CTAs that align to the brand palette. Replace links or copy directly in the files as needed.

## Working with assets
Place hero or feature imagery in the `images/` directory. Reference them in the templates with `src="images/your-file.jpg"` so Maizzle copies them into the build output. Update alt text for accessibility whenever you change imagery.

## Build and export
1. Install dependencies: `npm install`.
2. Build production-ready HTML: `npm run build`.
3. Find the compiled files in `build_production/` with CSS inlined and assets copied to `build_production/images/`.

## Mailchimp upload notes
- Mailchimp accepts either pasted HTML or a ZIP containing the compiled HTML and its asset folder. Upload the HTML files from `build_production/` and include the `images/` directory if you use local assets.
- If Mailchimp hosts your images, swap `src` values to absolute URLs before uploading.
- Test with Mailchimp’s preview and inbox rendering tools to confirm button styles, spacing, and line heights remain intact across clients.
