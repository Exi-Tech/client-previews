# Client preview workflow

This is the shared operating guide for Ahmad, Hayiqa, Haroon and Aveen. Give Codex the lead rows and the employee name, then ask it to follow this file from research through live verification.

## 1. Research before designing

1. Ignore dummy CRM emails and unrelated personal data.
2. Search the exact business name, address and phone on Google/web search.
3. Open the supplied website or booking link. Confirm whether it belongs to the whole business, one employee, or an outdated listing.
4. Search for the business's official Instagram and Facebook. Add a social link only when the name, location and branding clearly match. Record “not verified” when uncertain.
5. Resolve conflicting facts. Prefer a current first-party business/booking page for services and booking; use the supplied Google record for its current phone, address, hours, rating snapshot and Place ID unless stronger current evidence is found. Document every decision.
6. Use only images confirmed to belong to that exact business. Never use search-result images from similarly named businesses.

## 2. Select two templates

Read the local templates/README.md selection guide. Choose two templates that fit different strengths of the lead. Explain the choice in the client README. Never edit files inside templates/; copy and adapt them. The templates folder is local and ignored by Git.

## 3. Standard folder structure

```
Employee/client-slug/
  index.html                 # selector for both concepts
  README.md                  # sources and decisions
  assets/
    sources.json
    images, fonts, shared CSS
  template-one/index.html
  template-two/index.html
```

Use the existing employee capitalization. Use lowercase hyphenated client and template slugs. Keep all asset links relative so GitHub Pages works under /client-previews/.

## 4. Content rules

- Do not mention Exi-Tech. These are personal outreach previews.
- Mark the footer “Website concept · Not the official website.”
- Do not invent services, prices, staff, testimonials, awards or claims.
- Keep pricing and availability on the existing booking provider when those change by barber or date.
- Add `noindex,nofollow`; the repo and pages are still public.
- Booking, phone, maps and verified social links must point to the real business.
- If a template's live-hours feature could use the visitor's timezone, replace it with static verified hours or calculate in the business timezone.
- Logo graphics must use natural proportions (`width:100%; height:auto; object-fit:contain`). Photographs may use `object-fit:cover` only after their crop is visually checked.

## 5. Quality check before publishing

Check both concepts at 1440px, 390px and 320px widths. Confirm:

- no horizontal overflow, broken images, duplicate IDs, script errors or broken section links;
- logo and important subjects are not cropped;
- all original-template names, images, addresses, emails and copy are gone;
- Exi-Tech does not appear anywhere on client-facing pages;
- employee/client facts match sources.json;
- booking, call, directions, reviews and social links work;
- the concept selector opens both versions;
- master template hashes are unchanged.

After pushing, wait for GitHub Pages to finish and repeat the same checks on the live URLs. Inspect screenshots, not only automated pass/fail output. Add a cache-busting query only for internal rechecks; send clean URLs to leads.

## 6. Sending through social media

Social apps do not understand Markdown link syntax. Send plain URLs, each on its own line. Prefer the single concept-selector URL unless there is a reason to send both direct links.

Example:

```
Hey [Name], since I'd already put these concepts together, I thought I'd leave them here anyway:

https://exi-tech.github.io/client-previews/Employee/client-slug/

No need to reply—I'll leave it here. Wishing you and the business continued success!
```

## 7. Privacy and source records

Never commit raw lead tables, dummy emails, credentials, tokens or unrelated personal information. Each client README explains the public facts used and any conflict resolution. Each assets/sources.json records source URLs and the date checked.
