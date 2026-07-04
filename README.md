# Tamha

Tamha is a mobile first Design Component prototype for local lost item and missing person alerts. It lets a user draft a report, attach a simulated photo state, browse nearby sample posts, open a detail page, send a lead, call a contact number, and mark a post as found.

The Thai name means "to search for". The internal idea key was `แจ้งของหาย/คนหายในพื้นที่`.

## Important Safety Note

This is a prototype, not a live emergency or official missing persons system. The sample posts, distances, map, notifications, geolocation, and backend behavior are mocked. For a real missing child, elderly person, patient, or other urgent case, contact the proper authorities and use the national 1300 missing persons hotline where appropriate. Do not publish private or sensitive information without a lawful reason and consent where required.

## What Is Included

| File | Purpose |
| --- | --- |
| `Tamha.dc.html` | Runnable single file prototype with the main flow and local state. |
| `Tamha Overview.dc.html` | Screen overview board showing the major app states side by side. |
| `support.js` | Design Component runtime required by the HTML files. |
| `screenshots/` | Clean rendered screenshots for README preview and handoff review. |

## Main Prototype Flow

1. Open the app and review nearby alerts.
2. Choose a lost item or missing person report type.
3. Fill in title, last seen area, date or time, description, contact number, and optional reward.
4. Preview the report.
5. Publish it into the local browser demo feed.
6. Open a detail page, send a lead, call the listed number, or mark the post as found.

## Product Features

- Local feed filtered by all posts, missing people, lost items, and found posts.
- Missing person related screens surface a 1300 hotline call to action.
- Detail pages show a last seen area, sample map block, metadata, contact actions, and status controls.
- Alerts and My Posts screens are included for the prototype flow.
- English and Thai UI copy are available through the language toggle.
- User created demo posts are stored in `localStorage` under `tamha_posts_v1`.

## Screenshots

| App Home | Design Overview |
| --- | --- |
| ![Tamha app home](screenshots/tamha-app-home.png) | ![Tamha design overview](screenshots/tamha-design-overview.png) |

## Running Locally

Open `Tamha.dc.html` directly in a modern browser. No install or build step is required. The prototype is designed for a mobile width around 390 to 460 px.

## Data And Prototype Limits

- Sample people, item reports, phone numbers, locations, distances, and alerts are fictional demo data.
- The app does not send notifications, upload photos, perform geolocation, or connect to Supabase.
- The photo picker is a simulated attached state for design review.
- `tel:` links open only on devices and browsers that support dialing links.

## Handoff Notes

For production, connect verified moderation, reporting, privacy controls, location permissions, backend storage, audit logging, and abuse prevention before collecting real reports.
