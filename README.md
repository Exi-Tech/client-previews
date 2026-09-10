# Client previews

One GitHub Pages site, multiple static client concepts. Publish from main / root; .nojekyll bypasses processing. Every push updates the shared site.

## Standard structure

Employee/client-slug/index.html is the client concept selector. Employee/client-slug/template-slug/index.html is a preview. Employee/client-slug/assets/ holds that client's shared photos, fonts and styles. Preserve existing employee names and case: Ahmad, Hayiqa, Haroon, Aveen. Client and variant names use lowercase hyphenated slugs.

The local templates/ folder (including its README selection guide) is ignored and must never be force-added. Clone users need their own local template copies. Original templates stay unchanged; adapt client copies only. Use relative asset paths so all pages work below /client-previews/.

Do not commit raw CRM exports, dummy emails, unrelated personal details, credentials or tokens. Concept pages use noindex, which is not access control: this repository and its deployed assets are public. The root deliberately has no client directory.

## Publishing checklist

Verify client facts and photo sources. Check both mobile and desktop, booking/phone/maps links, keyboard access, image loading and absence of template business leftovers. Stage explicit client paths. Commit and push main, wait for Pages, then verify the deployed pages. No separate deployment per client. Booking stays at the business's existing provider.
