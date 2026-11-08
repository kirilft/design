# GDPR

Applies to every website with visitors in the EU. German law adds the TDDDG (cookies) and the DDG (Impressum).

## Cookie banner
- A site that sets non-essential cookies, writes non-essential data to `localStorage`, or loads third-party content needs a consent banner. If it's missing, add it.
- Essential means needed for the site to work: login session, cart, the consent choice itself. Analytics, ads, and embeds are not essential.
- Nothing non-essential runs before the visitor agrees.
- "Reject" is as easy and as visible as "Accept": same level, same size. No pre-ticked boxes.
- The visitor can change the choice later, through a link in the footer.
- The banner sits above everything else (see [layout.md](layout.md)) and follows [accessibility.md](accessibility.md).

## Third-party content
- Fonts: self-host them. Loading from Google's servers sends visitor IPs to Google.
- Embeds (YouTube, Google Maps, social media): load them only after consent. Show a placeholder with a "Load content" button until then.
- Analytics: only after consent, or a cookieless tool that stores no personal data.
- CDNs: self-host scripts and styles where possible.

## Required pages
Link these from the footer of every page:
- **Privacy policy:** what data is collected, why, how long it's kept, who receives it, and the visitor's rights.
- **Impressum** (Germany, Austria): name, address, and contact of the operator. Required for business and commercial sites.
- **Licenses:** see [licensing.md](licensing.md).

## Forms
- Ask only for the data you need. Mark required fields.
- Link the privacy policy next to the submit button.
- Use HTTPS on every page.
