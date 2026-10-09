# SCC updates

[Back to the docs](README.md)

## 3.4.3 — October 8, 2026

- Fixed **Force full refresh** skipping the Wiki's current game version. SCC now checks that version before reloading the related catalogs.
- Kept a full-refresh request queued when an automatic pass is already running. Repeated requests are combined so they don't start duplicate full refreshes.
- Added per-resource refresh failures, the last successful fetch, and when automatic refresh is due to my maintenance dashboard. The page updates while a refresh runs.
- Moved older fallback caches into a separate section so they don't look like active resources that failed to refresh. Previous data stays available during provider outages.

## 3.4.2 — October 8, 2026

- Fixed navigation buttons becoming unresponsive after a few activity changes. Quick clicks now update the same panel in order.
- Fixed private-panel Close and search-form returns. Keep result retains the current card without its controls.
- Reworded the docs in my own voice, including support, reports, maintenance, privacy, and contact details.

## 3.4.1 — October 8, 2026

- Added direct Home buttons for trade runs, item searches, and ship browsing, plus activity navigation from Help.
- Added private Settings access from result menus while keeping a public result usable.
- Kept navigation and cleanup controls available after an empty search or unavailable lookup.
- Connected community note search results to full notes and Back navigation, with access limited to the current server.
- Added pages for crew activity lists and routes back from jobs and earnings. Personal crew panels refresh after participation changes; closed activities keep navigation with participation controls disabled.
- Split long ship details and notes into pages, retaining their information within Discord's limits. Back returns to the filtered ship list.
- Corrected crafting material estimates for recipes that produce several items per craft, and mining trip estimates for fractional cargo amounts.
- Protected replacement and kept results from older cleanup timers, and refreshed interaction handling during continued browsing.
- Added visible Wiki API credit and source links to ship lists. Disabled server-only controls in direct messages.

## 3.4.0 — October 8, 2026

- Added UEX player sellers to weapon, material, and recipe-ingredient browsing. Player listings and NPC shop prices are shown separately.
- Added seller/buyer filters for price, quality, location, currency, and unit. Listings open on UEX so you can contact the trader there.
- Made searches and topic changes reuse the current menu instead of filling the channel with replies.
- Added **Close**, **Keep result**, and automatic cleanup for temporary menus. Shared hubs and crew boards stay in place.
- Made search, settings, and crew cards more consistent, and fixed Back navigation in ship and marketplace results.
- Added **Home → What’s new** for patch notes.

## 3.3.0 — October 8, 2026

- Added `/item`, `/blueprint`, and `/menu` as browsing entry points, while keeping the existing shortcuts.
- Connected Trade, Mining, Ships, and Crafting through activity menus, related-result selectors, and Back buttons.
- Added ingredient browsing so you can move from a recipe into materials, mining guidance, shops, and sources.
- Added Wiki article/search links, original Wiki data links, UEX price references, and public RSI source links.
- Split long recipes and results into pages. Improved exact matching and made ambiguous results clearer.
- Kept Wikelo barter separate from blueprint crafting, and preserved private/public preferences and server permissions.

## 3.2.0 — October 8, 2026

- Added first-run setup and personal/server defaults for language, pledge currency, ship budget, and private/public replies.
- Added highlighted activity sections, button-driven searches, and ship browsing by role and budget.
- Added `/settings`, `/config setup`, and reusable `/config panel` channel hubs.
- Added saved controls for SCC's own status and activity. I manage these because they affect SCC across every server.
- Used actual provider prices for the selected pledge currency, with labelled fallbacks when a source lacks that currency. In-game prices remain in aUEC.
- Improved optional account-linking explanations and protected personal public menus from other people changing them.
- Added translated navigation, setup, reply choices, and command descriptions across ten supported languages.

## 3.1.0 — October 8, 2026

- Added optional display of verified RSI handles and the last verification date on crew boards. Members control this separately for each server.
- Added weekly activities with local-timezone scheduling and fresh signups, jobs, and earnings records for each session.
- Added private activity reminders, delivery status, and cancellation when a member leaves or an activity closes.
- Added tracking and retries for crew-board updates, including changes to identity-display permissions.
- Added translations for the new command descriptions and preserved existing community records during the update.

## 3.0.2 — October 8, 2026

- Added encrypted recovery backups, off-device copies, and restoration checks.
- Added readiness checks for Discord, the database, and scheduled tasks, with separate warnings for provider outages and backup freshness.
- Replaced the older updater with a checked update-and-recovery process.
- Kept reports local for my review. Added editable, redacted previews before I choose to forward a report to a private repository.
- Improved credential redaction in support bundles and report exports, including Citizen iD client identifiers.
- Updated maintenance, security, backup, and recovery guidance.

## 3.0.1 — October 7, 2026

- Updated StarCitizen-API support to its v2 authentication and paginated ship catalog, with cached lookups and bounded retries.
- Added optional Citizen iD sign-in, verified RSI account linking, unlinking, and private `/identity` controls.
- Kept production and staging identities separate; staging profiles do not grant live verification.
- Added optional Discord sign-in to my private maintenance dashboard.
- Improved sign-in validation, login throttling, and protection for account forms and sessions.

## 3.0.0 — September 30, 2026

- Added guided task menus and grouped related commands under Trade, Ships, Cargo, Crafting, and Inventory.
- Added server-scoped activities, crew roles, capacity checks, jobs, and persistent crew boards.
- Added activities from crafting plans, saved material requirements, shortage jobs, and review notices when source data changes.
- Added shared material reservations, adjustment history, verification dates, and release of unused reservations when an activity closes.
- Added refinery-job tracking and reminders, plus rescue and escort requests with responder and expiry controls.
- Added income/expense ledgers, equal or weighted crew splits, settlements, and manual paid markers for in-game earnings.
- Added server feature switches and private maintenance controls.
- Corrected trade supply/demand handling, stock allocation by quality, and payout rounding. Improved route selection responsiveness.
- Preserved existing community records during the database update and kept records isolated between servers.

## 2.4.1 — September 29, 2026

- Added mining-resource, laser, modifier, loadout, sale, and trip-planning tools.
- Added refinery-method rankings, station yield bonuses, and capacity guidance.
- Added mission search, qualification paths, and mining-mission workflows.
- Added salvage-ship, sale, and cargo-trip planning.
- Added cached public citizen, organisation, and starmap lookups through StarCitizen-API, plus ship/starmap fallback data.
- Connected crafting ingredients to mining methods, locations, and sale information.
- Made autocomplete suggestions fit the selected operation, including shops, terminals, mining ships, inventory, alerts, and notes.
- Expanded `/start` and `/help`, and moved several raw data commands into more useful activity tools.
- Restricted shared source refreshes to me and improved handling of expected permission errors.
- Added command validation during the build so an invalid update can be rejected before deployment. Corrected the package-import issue from the superseded 2.4.0 package.

### Earlier changes included in the September 29 update

Versions 2.1.0 through 2.3.2 were installed together with 2.4.1. Separate release dates weren't recorded for these entries.

#### 2.3.2

- Fixed MOLE Teach's Special matching to use the standard MOLE family rather than the retired Carbon edition.
- Moved Teach's Ship Shop prices to the dealer-special edition, keeping them separate from the standard ship.
- Added an origin fallback for special editions without a current UEX price.
- Separated mining-ship cargo space from ore capacity and corrected reversed crew bounds.
- Added exact cargo-box limits from Wiki records and a catalog fallback during an upstream version failure.
- Fixed overlong translated cargo-command descriptions blocking command synchronisation.

#### 2.3.1

- Combined UEX and Wiki ship catalogs into one identity index, including Wiki-only and Teach's Special variants.
- Routed dealer-modified purchase and rental records to the correct editions and repaired missing ship identifiers through exact matches.
- Fixed ship descriptions that displayed raw data instead of readable text.
- Kept exact autocomplete selections from being matched again to another model.
- Added supported container sizes, cargo-fit guidance, and current/historical labels for purchase and rental records.
- Added cached Wiki vehicle data with a UEX fallback.

#### 2.3.0

- Added ship variant, edition origin, purchase, rental, and pledge information.
- Added Teach's Special configuration and Levski/Nyx source information.
- Added ship variants, comparison, and shop tools.
- Added rental-price caching, data freshness labels, and CStone/Wiki verification links.

#### 2.2.3

- Made exact ship autocomplete selections return the selected model and improved partial-name searches.
- Added published blueprint unlock-mission qualifications, including faction, standing, prerequisite contracts, legality, and release status.
- Added source links and game-data version labels to blueprint results.

#### 2.2.2

- Fixed valid blueprint unlock missions displaying as “Unknown.”
- Improved grouped mission results, duplicate counts, reward scope, and fallback information.
- Made it clear when an unlock is required but the current data does not publish its mission source.

#### 2.2.1

- Corrected Wiki blueprint pagination, deduplicated results, and refreshed the blueprint cache.
- Added support for the source's updated output-name and material-quantity fields.

#### 2.2.0

- Added `/start` and categorised `/help` guides for trade, crafting, ships, community tools, and server administration.
- Expanded language support to Russian, Korean, Simplified Chinese, and Traditional Chinese.
- Added translated command and option descriptions, with English fallback.
- Added autocomplete for commodities, terminals, ships, items, locations, blueprints, materials, inventory records, notes, alerts, and settings.
- Made empty autocomplete fields show useful examples and updated SCC's activity to point people to `/start`.

#### 2.1.0

- Added community notes with categories, tags, patch/version labels, references, search, editing, deletion, and member verification.
- Added personal/server language preferences, Discord-language detection, and the first six language catalogs.
- Added usage totals and server opt-out. Command analytics exclude user IDs, command arguments, and message content.
- Added official RSI service-status lookups and change notifications.
- Added private maintenance views for notes, analytics, and status subscriptions, and improved update/support validation.

## 2.0.0 — Release date not recorded

- Rebuilt SCC around shared services for Discord and private maintenance tools.
- Added health checks, logs, backups, inventory, a crafting planner, and alerts.
- Added Wiki blueprint data and the UEX API 2.0 integration.
- Replaced blocking network calls with asynchronous requests, timeouts, retries, and concurrency limits.
- Consolidated background refreshes into a managed scheduler with refresh locking.
- Isolated community records, inventory, preferences, blueprint ownership, and alerts between servers.
- Improved private-file exclusions, container permissions, log rotation, database reliability, and update/migration tools.
- Removed unsafe live reload behaviour and added controlled import of older records.

Use the [current command reference](COMMANDS.md) for today's commands and options. Read the latest patch notes in Discord under **Home → What’s new**.
