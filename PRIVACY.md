# BreakIt Privacy Policy

Last updated: September 9, 2026. Applies to BreakIt v0.1.0.

## What BreakIt does

BreakIt is a Chrome extension for testing interface durability with text expansion, pseudo-localization, right-to-left (RTL) direction, and suspected overflow highlighting. See how your UI breaks before your users do.

All extension processing runs locally in your browser. BreakIt starts working on the current webpage when you open the extension. While stress modes are active, it can continue processing new or updated page content after the popup closes, until you reset the page or reload or navigate away.

## Data handling

BreakIt reads visible DOM text and element geometry to apply UI stress tests and identify potential layout failures. Original text, DOM node references, active settings, and layout measurements are held temporarily in page-local memory to support testing and Reset. Only settings and the potential issue count are returned to the extension popup inside Chrome; page text is not returned to the popup.

BreakIt does not collect browsing history, page text, personal information, or usage data for persistent storage or transmission. No page contents or other information are sent by the extension to the developer or anyone else. There is no analytics, telemetry, account, cloud storage, remote code, or external service. The extension makes no network requests and uses no cookies or persistent extension storage.

Reset clears retained original text and removes injected styles and highlights, while preserving newer text edits made by the website. Reset also rescans the page to update the potential issue count; it does not unload the bundled page logic. Reloading or navigating away discards page-local state.

## Permissions

- **activeTab** grants temporary access to the tab where you invoke BreakIt.
- **scripting** allows BreakIt to run its bundled page logic in that tab.

No broad host permissions are requested. Access to local demo files requires you to enable Chrome's separate file URL access setting.

## Websites you test

BreakIt does not submit forms or intentionally modify application data. It temporarily changes rendered DOM content. The website's own scripts may independently observe those changes and react to or transmit them under that website's own privacy practices. BreakIt does not control those scripts; the website's own privacy policy applies to its activity.

## This policy page

The extension's local-only behavior is separate from visiting this policy on a website. Loading the hosted policy page requires a normal web request to its hosting provider, which may process request information under its own privacy policy. This page includes no scripts, analytics, tracking pixels, or third-party embedded resources.

## Contact and support

Contact/support: [Publisher to add a monitored support email address or public support URL before publication.]
