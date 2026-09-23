# LazyDeals Privacy Policy

_Last updated: September 23, 2026_

LazyDeals is a Microsoft Edge and Google Chrome extension that monitors PC game prices and notifies users when their chosen price targets are met. This policy describes how LazyDeals V1 handles data.

## Information stored by the extension

LazyDeals stores the information needed for price monitoring:

- tracked game identifiers and price targets;
- preferred stores and the selected pricing mode;
- cached game, store, and price information;
- current-deal and notification state; and
- timing and cooldown information for background checks.

User choices, such as the watchlist and targets, use browser-managed extension sync storage. If browser synchronization is enabled, the browser provider may synchronize that information according to the user's browser and account settings. Reconstructible caches and runtime state use local extension storage.

LazyDeals does not require a LazyDeals account and does not operate a backend that receives or stores this extension data.

## Requests to pricing providers

LazyDeals makes HTTPS requests from the user's browser to the following independent services when needed for search or price monitoring. Like other web requests, these services may receive the user's IP address, request headers, timestamps, and the information described below.

### CheapShark

LazyDeals uses CheapShark for its game and store catalogs, game search, game information, and All Stores prices. Requests may contain search text entered by the user or CheapShark game identifiers.

Saved price targets and preferred-store rules are evaluated inside the extension; LazyDeals does not send those saved rules to CheapShark for target evaluation.

[Visit CheapShark](https://www.cheapshark.com/).

### Steam Store

In Regional mode, LazyDeals requests Steam Store price information when a tracked game has a Steam App ID. These requests contain the Steam App ID needed for the lookup.

LazyDeals evaluates the saved Regional target inside the extension. It uses the price and currency returned by Steam and does not convert currencies or send the saved target value as part of the price lookup.

[Read Valve's privacy policy](https://store.steampowered.com/privacy_agreement/).

## How information is used

LazyDeals uses this information to maintain the watchlist and settings, retrieve game prices, compare prices with saved targets, display current deals, pace background checks, and generate price notifications.

LazyDeals does not sell user data. V1 does not include analytics, telemetry, personalized advertising, or a LazyDeals-operated account service.

## Browser permissions and browsing activity

LazyDeals requests extension storage, alarms, notifications, and access to the CheapShark and Steam Store hosts used by its features.

LazyDeals does not request browsing-history, cookies, geolocation, active-tab, page-scripting, or general website-access permissions. It does not inspect the content of webpages the user browses.

## Retention and user controls

Users can edit or remove tracked games and their targets in LazyDeals. Removing a tracked game removes its saved tracking configuration and triggers best-effort cleanup of related cached and runtime information.

Local extension data is managed by the browser and is normally removed from that browser when the extension is uninstalled. Synced data is additionally subject to the browser provider's synchronization and account settings. Users can manage extension data through their browser's available controls.

## Security and third-party services

LazyDeals communicates with CheapShark and the Steam Store over HTTPS. No LazyDeals-operated server receives the watchlist, targets, preferences, cached prices, or runtime state in V1.

CheapShark, Steam, and the browser's synchronization service operate independently of LazyDeals and may handle information according to their own policies. LazyDeals does not control their availability or data-retention practices.

## Changes to this policy

This policy will be updated if LazyDeals materially changes its data handling—for example, by adding another pricing provider, analytics, accounts, or a backend.

## Contact

For privacy questions or support, email: lazydeals.help@outlook.com