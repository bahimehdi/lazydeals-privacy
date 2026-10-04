# LazyDeals Privacy Policy

_Last updated: October 4, 2026_

LazyDeals is a browser extension for Chrome and Microsoft Edge that tracks PC game prices and notifies users when configured price targets are met.

This policy describes the data LazyDeals handles, including the optional Steam wishlist import.

## Data LazyDeals stores

LazyDeals stores the information needed to provide its price-tracking features, including:

- tracked game identifiers;
- All Stores and Regional price targets;
- preferred store selections;
- the selected pricing mode;
- cached game and store metadata;
- recent provider price data;
- notification and current-deal runtime state; and
- request/check timing state used to pace background checks.

The optional discovery-alert preference is stored in browser sync storage. Reported free-to-keep offer snapshots, offer IDs already seen, notification routing, and discovery refresh/cooldown state are stored locally on each device. These offer records are separate from your tracked games and targets.

If you use Steam wishlist import, LazyDeals also stores your Steam wishlist Share URL on that device, including its private `st` token if present. It stores the last completed view's Steam App IDs and import status, plus a temporary import draft and progress. These values stay in local extension storage; the Share URL and token are not copied to browser sync storage. The Share URL is retained until you replace or remove it. Removing it also clears the local view snapshot and unfinished import job, but does not remove tracked games or targets.

Durable user settings are stored with the browser extension storage API. Some durable settings use browser-managed sync storage.

When browser synchronization is enabled, the browser may synchronize supported extension data across browsers signed in to the same browser account.

Caches and runtime state use local extension storage. The optional saved Share link, completed-view snapshot, and unfinished import draft are also local, but are not reconstructible without the link or a new import.

LazyDeals does not require a LazyDeals account and does not operate a LazyDeals backend that receives or stores this extension state.

## Data sent to pricing providers

LazyDeals contacts third-party pricing services only when needed to provide its game-search and price-monitoring features.

As with normal HTTPS requests, those providers may receive ordinary network and request metadata such as the requesting IP address, request headers, and timestamps according to their own data-handling practices.

### CheapShark

LazyDeals uses CheapShark for:

- the game catalog;
- the store catalog;
- game search;
- game metadata; and
- All Stores pricing data.

Requests may include:

- game search text entered by the user; and
- CheapShark game identifiers needed to retrieve game or pricing information.

Saved target prices and preferred-store rules are evaluated inside the extension and are not sent to CheapShark as part of LazyDeals target evaluation.

More information about CheapShark is available at:

<https://www.cheapshark.com/>

### Steam

LazyDeals uses the Steam Store for Regional pricing when a tracked CheapShark game has a Steam App ID.

Requests include the Steam App IDs needed to retrieve current Steam Store pricing information.

When you start an import or manually select Update, LazyDeals requests the pasted or saved Steam wishlist Share URL from Steam. A private Share token in that URL is sent to Steam as part of the request. LazyDeals uses App IDs from that view to check release and regional-price availability. It does not send the Share URL or its token to CheapShark; only App IDs are used for CheapShark matching. Wishlist import does not automatically poll your Steam wishlist.

Saved Regional target values are evaluated inside the extension and are not sent to Steam as part of the price lookup.

LazyDeals uses the price and currency returned by Steam and does not perform currency conversion.

Valve's privacy policy is available at:

<https://store.steampowered.com/privacy_agreement/>

### FreeToKeep.GG

LazyDeals uses [FreeToKeep.GG](https://freetokeep.gg/) to show reports of normally paid PC games temporarily offered for free on Epic Games Store, Steam, and GOG. The extension checks its public offer API when a discovery refresh is due, independently of your watchlist or selected pricing mode. Requests do not include your tracked games, target prices, or Steam wishlist Share URL. Ordinary HTTPS request metadata, including your IP address, may be received by FreeToKeep.GG.

Offer reports can be late, wrong, withdrawn, or unavailable for your region or account. LazyDeals does not independently verify each storefront claim; open an offer and check it before relying on it. The card's “View reported offer” action opens FreeToKeep.GG's offer page, which may link onward to a storefront. Offer images, when present, load from external HTTPS image hosts; those hosts may receive normal request metadata such as your IP address. LazyDeals sends no referrer with these image requests.

## Browser-managed synchronization

LazyDeals uses the browser's extension sync storage for durable settings.

If browser synchronization is enabled, the browser provider may synchronize supported extension data according to the user's browser and account sync settings.

LazyDeals does not operate or control the browser provider's synchronization service.

## Permissions and browsing data

The extension requests only the permissions required for:

- extension storage;
- scheduled alarms;
- native notifications; and
- access to the CheapShark and Steam Store hosts used by its pricing features; and
- access to FreeToKeep.GG for reported free-to-keep discovery.

LazyDeals does not request permissions for:

- browsing history;
- cookies;
- geolocation;
- browser identity;
- active-tab access;
- page scripting;
- content scripts; or
- general access to websites the user visits.

LazyDeals does not inspect the content of webpages the user browses.

## Analytics, telemetry, and advertising

The current extension does not use analytics or telemetry services and does not include personalized advertising.

LazyDeals does not sell user data.

## How data is used

Data handled by LazyDeals is used only to provide the extension's disclosed functionality, including:

- maintaining the watchlist and saved targets;
- remembering preferred stores and the active pricing mode;
- retrieving game and price information;
- evaluating whether a configured target has been met;
- displaying current deals;
- pacing automatic and manual checks; and
- importing a Steam shared wishlist view and retaining local progress for a user-requested Update; and
- generating price notifications; and
- showing reported 100%-off offers and sending optional discovery notifications.

## Data retention and user control

Users can edit or remove tracked-game configuration from LazyDeals.

Users can remove the saved Steam Share link and associated local import state from the import panel. Cancelling an import removes its draft. Games already confirmed into the LazyDeals watchlist remain tracked until explicitly removed, even if they later disappear from the Steam wishlist.

Removing a tracked game removes that game's durable tracking configuration and triggers best-effort cleanup of related reconstructible runtime state.

Local extension storage is managed by the browser and is removed from that browser when the extension is uninstalled.

Data stored through browser-managed sync storage is additionally subject to the browser provider's synchronization and account settings.

Users can also clear extension data through the browser's own extension/data management features where supported.

## Security

LazyDeals communicates with its configured pricing providers over HTTPS.

No LazyDeals-operated server receives the watchlist, targets, preferences, cached provider state, or extension runtime state in the current version.

## Third-party services

LazyDeals depends on CheapShark and the Steam Store for external catalog or pricing information, and on FreeToKeep.GG for reported 100%-off offers.

Those services operate independently of LazyDeals and may process network/request information according to their own terms and privacy practices.

LazyDeals does not control third-party provider availability, retention practices, or privacy policies.

## Changes to this policy

This policy should be updated whenever LazyDeals changes what data it handles or introduces features such as:

- a LazyDeals backend or account system;
- analytics or telemetry;
- advertising;
- additional pricing or discovery providers;
- new categories of user data; or
- materially different synchronization or storage behavior.

## Project

LazyDeals source code and project information:

<https://github.com/bahimehdi/lazydeals>

## Contact

For privacy questions or support, email: lazydeals.help@outlook.com
