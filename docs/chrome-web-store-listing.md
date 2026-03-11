# Chrome Web Store Listing Draft

Use this as a template for your Chrome Web Store submission.

## Extension name

hetu - Hide SSN on Finnish authentication sites

## Short description

Hides visible Henkilotunnus values on selected Finnish authentication pages using local CSS.

## Detailed description

hetu - Hide SSN on Finnish authentication sites is a minimal privacy-focused extension for Chrome.

It applies local CSS rules on selected authentication pages to hide visible Finnish personal identity code values (Henkilotunnus) from on-screen display.

### Key points

- Pure CSS implementation (no JavaScript runtime logic)
- No data collection or tracking
- No remote code
- No external network requests
- URL-scoped behavior only on explicitly configured pages

### Supported URLs

- `https://userapi2.danskebank.com/prod/external/ftn/idp-oidc/connect/sign-in*`
- `https://tunnistautuminen.suomi.fi/idp/profile/SAML2/Redirect/SSO*`

## Privacy practices (store form guidance)

- Data collection: No
- Data sale: No
- Data sharing with third parties: No
- Data usage for personalization/ads: No
- Authentication data handling: None

Reference policy: `PRIVACY_POLICY.md`

## Category suggestion

Productivity

## Single purpose statement

This extension hides visible Finnish personal identity code values on specific login pages for improved shoulder-surfing privacy.

## Store assets checklist

- 128x128 icon (`icons/icon128.png`)
- Screenshots (at least 1, recommended 3)
- Promotional images (optional)

## Notes

- Ensure screenshots do not contain real personal data.
- Keep listing text aligned with actual permissions and behavior.
