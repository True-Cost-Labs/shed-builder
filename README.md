# Shed Builder — 3D Shed Designer

A free, single-file 3D shed builder that runs entirely in the browser. No build step, no server, no dependencies — open `index.html` and it works.

Pick a style, size it, paint it, place doors and windows, then orbit the build in true 3D — or step inside and walk through your own layout. Includes a blueprint mode (drag and resize walls, doors, windows, rooms and additions like a loft, workbench, shelving, electrical, insulation and porch), a clean image export of your design, printable quote sheets and PDF planning packs (blueprint sheet, a size-fitting decision kit, and a site-prep + delivery checklist).

## Make it yours (2 minutes)

Everything a dealer or seller needs to change is in one place each:

1. **Your phone number** — find-and-replace `YOUR-PHONE` with your number (it appears in the call/text buttons and quote sheets).
2. **Your pricing** — near the top of the script, the `PRICING` block holds the whole payment formula:

   ```
   monthly = ((list x (1 - discountPct)) + docFee + deliveryFee) x (1 + taxRate) / monthlyDivisor
   ```

   The defaults are neutral (no discount, no fees, no tax), so the monthly shown is simply list ÷ monthlyDivisor until you set your own numbers. A worked example with one Washington dealer's rent-to-own math is in the comment right above the block.
3. **Your name** — the title and headings say "Shed Builder"; change them to your business name wherever they appear.

The shed catalog (styles, sizes, list prices, colors, options) is plain data in the same file — edit the `CATALOG` tables to match what you sell.

## Host it free with GitHub Pages

In your repository: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / root**. Your builder is then live at `https://<your-name>.github.io/<repo>/`.

## License

Free edition — free for personal and commercial use for your own business. See `LICENSE.md`. A Pro edition with in-page pricing settings, your own branding throughout, and lead capture is separate.

Built by Thomas Wolf (True-Cost-Labs).
