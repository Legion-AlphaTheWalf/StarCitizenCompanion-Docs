# Command reference

[Back to the docs](README.md)

These are the **129 commands available in SCC 3.4.3**. Start with `/start` if you'd rather browse menus. In Discord, type a command to see its options and autocomplete suggestions.

Options marked **required** must be filled in. Replace `<value>` with your own choice; don't type the angle brackets.

**Manager** commands need Manage Server permission; I also have access as SCC's maintainer. **Maintainer** commands are restricted to me (**AlphaTheWalf**). Other actions may depend on the server's enabled features, channel permissions, and who owns the activity or record.

Settings, reports, account linking, and reminders stay private. Ordinary searches follow your reply preference; crew and support boards are shared in their channel.

## Jump to a family

- [General](#general)
- [analytics](#analytics)
- [cargo](#cargo)
- [config](#config)
- [craft](#craft)
- [debrief](#debrief)
- [identity](#identity)
- [inventory](#inventory)
- [language](#language)
- [ledger](#ledger)
- [lookup](#lookup)
- [mining](#mining)
- [mission](#mission)
- [note](#note)
- [ops](#ops)
- [refinery](#refinery)
- [salvage](#salvage)
- [ship](#ship)
- [status_watch](#status_watch)
- [support](#support)
- [trade](#trade)
- [trade_alert](#trade_alert)

## General

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/blueprint` | Explore a blueprint or open the Crafting menu | `query:<value>` — Blueprint or finished item; leave empty to open the Crafting menu | — |
| `/bug` | Send me a private report about an SCC problem | `description:<value>` **required** — What happened, what you expected, and which command was involved | — |
| `/fuel_best` | Compare the cheapest cached hydrogen or quantum fuel locations | `fuel_type:<value>` **required** — Choose hydrogen fuel or quantum fuel | — |
| `/help` | Browse SCC features, examples, and command categories | `category:<value>` — Choose a feature area to see its most useful commands | — |
| `/item` | Explore an item, its ingredients, shops and sources, or open the menu | `query:<value>` — Item or material name; leave empty to open the Crafting menu | — |
| `/item_find` | Find where an item is sold and compare cached purchase prices | `query:<value>` **required** — Select or type a weapon, armor, component, consumable, or other item | — |
| `/ping` | Check SCC's connection and Discord response time | None | — |
| `/privacy` | See exactly what SCC stores, excludes, and keeps server-isolated | None | — |
| `/report_data` | Privately flag an incorrect Star Citizen value, source, or location | `subject:<value>` **required** — Ship, item, mission, resource, terminal, or command with bad data<br>`correction:<value>` **required** — What SCC showed, what you believe is correct, and any source link | — |
| `/reports` | Review recent private bug reports and suggestions | `report_id:<value>` — Open a report's redacted preview before optional GitHub forwarding | Maintainer |
| `/rsi_status` | Check official Star Citizen platform and game service status | None | — |
| `/settings` | Choose your language, ship budget, pledge currency, and reply privacy | None | — |
| `/start` | Start here with guided buttons for SCC's most useful features | None | — |
| `/status` | Show Discord, provider, cache, RSI, and dashboard health | None | — |
| `/suggest` | Privately suggest a new SCC feature or improvement | `suggestion:<value>` **required** — Describe the feature and how players or servers would use it | — |
| `/sync_commands` | Resync SCC slash commands and translations with Discord | None | Maintainer |
| `/update` | Refresh SCC's shared UEX, Wiki, and reference caches | `force:<value>` — Refresh even when the current cache is still considered fresh | Maintainer |
| `/where` | Find terminals, cities, moons, planets, and their parent locations | `query:<value>` **required** — Select or type a terminal or location name | — |

## analytics

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/analytics global` | Show global anonymous command totals | `days:<value>` — Number of days to summarize, from 1 to 365 | Maintainer |
| `/analytics server` | Show private anonymous command totals for this server | `days:<value>` — Number of days to summarize, from 1 to 365 | Manager |
| `/analytics set` | Enable or disable optional anonymous analytics for this server | `enabled:<value>` **required** — Whether this server allows anonymous command totals | Manager |

## cargo

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/cargo capacity` | Quickly check the cached cargo capacity of a ship | `ship:<value>` **required** — Select or type the ship whose cargo capacity you need | — |
| `/cargo fit` | Check ship and terminal container-size compatibility for a cargo route | `ship:<value>` **required** — Select the exact ship or vehicle carrying the cargo<br>`buy_terminal:<value>` **required** — Origin terminal where the cargo is loaded<br>`sell_terminal:<value>` **required** — Destination terminal where the cargo is unloaded<br>`commodity:<value>` — Optional commodity for terminal-specific container reports<br>`scu:<value>` — Optional amount to pack; defaults to the ship's cached capacity | — |

## config

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/config features` | Choose which optional community workflows this server uses | `feature:<value>` — The optional feature to configure<br>`enabled:<value>` — Turn this feature on or off in this server | Manager |
| `/config get` | List advanced SCC settings saved for this server | None | Manager |
| `/config panel` | Post a reusable SCC button panel in this server channel | None | Manager |
| `/config presence` | Change SCC’s global Discord status and activity text | None | Maintainer |
| `/config set` | Set one advanced server-specific SCC value | `key:<value>` **required** — Setting name; suggestions show supported common keys<br>`value:<value>` **required** — New text value for this server | Manager |
| `/config setup` | Set server defaults for SCC language, ship budget, currency, and reply privacy | None | Manager |

## craft

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/craft blueprint` | Look up a crafting blueprint, ingredients, time, and unlock status | `query:<value>` **required** — Select or type the item or blueprint you want to craft | — |
| `/craft menu` | Open the connected SCC activity menu | None | — |
| `/craft own` | Record a crafting blueprint that you own for this server's planners | `query:<value>` **required** — Select or type the blueprint you personally own | — |
| `/craft owners` | See which members have recorded ownership of crafting blueprints | `member:<value>` — Optional member whose recorded blueprints you want to view | — |
| `/craft plan` | Compare a blueprint's requirements with this server's shared inventory | `query:<value>` **required** — Select or type the item or blueprint you want to produce<br>`quantity:<value>` — How many finished items you want to produce | — |
| `/craft sources` | Turn blueprint ingredients into mining, gathering, and sale-location guidance | `query:<value>` **required** — Select the blueprint or finished item you want to source<br>`quantity:<value>` — Number of finished items you intend to craft | — |

## debrief

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/debrief add` | Record a crew success or a lesson learned | `kind:<value>` **required** — A success or something that went wrong<br>`description:<value>` **required** — What happened and what the crew learned | — |
| `/debrief count` | Count this server’s recorded successes or lessons | `kind:<value>` — Which kind of debrief to count | — |
| `/debrief list` | Read recent successes or lessons learned in this server | `kind:<value>` — Which debriefs to show | — |

## identity

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/identity display` | Choose whether your verified RSI handle appears on this server’s crew boards | `enabled:<value>` **required** — Show your RSI handle in this server, or hide it | — |
| `/identity link` | Connect your linked Discord and RSI accounts through Citizen iD | None | — |
| `/identity status` | Show your own saved Citizen iD connection | None | — |
| `/identity unlink` | Remove your own saved RSI identity connection from SCC | None | — |

## inventory

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/inventory add` | Add crafting material to this server's shared inventory | `name:<value>` **required** — Select or type the material or item being stored<br>`quantity:<value>` **required** — How much is available<br>`unit:<value>` — Measurement unit such as units, SCU, cSCU, or kg<br>`quality:<value>` — Optional material quality value<br>`location:<value>` — Optional place where the material is stored | — |
| `/inventory history` | See additions, consumption, removals, and verification of shared stock | `item:<value>` **required** — Choose an inventory entry | — |
| `/inventory list` | List crafting materials recorded in this server's shared inventory | None | — |
| `/inventory menu` | Open the connected SCC activity menu | None | — |
| `/inventory remove` | Remove one suggested entry from this server's shared inventory | `entry_id:<value>` **required** — Select the inventory entry to remove | Manager |
| `/inventory verify` | Confirm that an inventory entry still matches the stock in game | `item:<value>` **required** — An inventory entry you own or manage | — |

## language

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/language reset` | Remove your override and automatically follow server or Discord language | None | — |
| `/language server_reset` | Remove the server override and use each member's Discord language | None | Manager |
| `/language server_set` | Set the default SCC response language for this Discord server | `language:<value>` **required** — Choose the default language for members without a personal preference | Manager |
| `/language set` | Override automatic detection with your personal SCC language | `language:<value>` **required** — Choose the language SCC should use for your responses | — |
| `/language show` | Show your personal, server, Discord, and resolved SCC language | None | — |

## ledger

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/ledger add` | Record actual income or an expense for your crew | `operation:<value>` **required** — An activity you lead<br>`kind:<value>` **required** — Income or expense<br>`amount:<value>` **required** — aUEC amount, with up to two decimal places<br>`description:<value>` **required** — What the money was earned or spent on | — |
| `/ledger paid` | Record a payment you have already made in game | `operation:<value>` **required** — An activity with a saved settlement<br>`member:<value>` **required** — The crew member you paid | — |
| `/ledger reopen` | Reopen an unpaid settlement to correct income, costs, or shares | `operation:<value>` **required** — An activity whose settlement has no recorded payments | — |
| `/ledger settle` | Save the final split and lock the ledger against accidental changes | `operation:<value>` **required** — An activity you lead with income, costs, and crew recorded | — |
| `/ledger show` | Preview crew earnings or view a saved settlement | `operation:<value>` **required** — Choose an activity | — |
| `/ledger void` | Correct the ledger by voiding an entry while preserving its history | `entry:<value>` **required** — Choose the incorrect ledger entry | — |
| `/ledger weight` | Adjust a crew member’s share; all members start with equal shares | `operation:<value>` **required** — An activity you lead<br>`member:<value>` **required** — Crew member whose share should change<br>`weight:<value>` **required** — Relative share from 1 to 100; 2 receives twice as much as 1 | — |

## lookup

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/lookup citizen` | Look up a public RSI citizen profile through the independent API cache | `handle:<value>` **required** — Public RSI handle to look up | — |
| `/lookup organization` | Look up a public RSI organization profile by Spectrum ID | `sid:<value>` **required** — Organization Spectrum ID, such as TEST or ORGNAME | — |
| `/lookup system` | Look up an independent cached RSI starmap system record | `system:<value>` **required** — Select or type a star system | — |

## mining

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/mining laser` | Inspect a mining laser's range, power, module slots, and modifiers | `laser:<value>` **required** — Select a mining laser or mining head | — |
| `/mining loadout` | Compare a laser and up to three mining modifiers against a rock profile | `laser:<value>` **required** — Mining laser or head<br>`modifier_1:<value>` — Optional first module or gadget<br>`modifier_2:<value>` — Optional second module or gadget<br>`modifier_3:<value>` — Optional third module or gadget<br>`rock_mass:<value>` — Optional scanned rock mass<br>`resistance:<value>` — Optional scanned resistance value<br>`instability:<value>` — Optional scanned instability value | — |
| `/mining menu` | Open the connected SCC activity menu | None | — |
| `/mining modifier` | Inspect a mining module or gadget and its published effects | `modifier:<value>` **required** — Select a mining module, consumable, or gadget | — |
| `/mining plan` | Build a simple mining trip plan around a resource, ship, and target amount | `resource:<value>` **required** — Resource you want to gather<br>`ship:<value>` — Optional mining or cargo ship for capacity planning<br>`amount_scu:<value>` — Optional target quantity in SCU<br>`priority:<value>` — Choose whether refining should favor yield, speed, or cost | — |
| `/mining resource` | Find how and where a mineable resource is obtained and sold | `resource:<value>` **required** — Select a mineral, gem, or mineable crafting material | — |
| `/mining sell` | Find the best cached locations to sell a raw mining resource | `resource:<value>` **required** — Select the raw mineral or gem to sell | — |

## mission

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/mission find` | Search current mission records by name and gameplay category | `category:<value>` **required** — Filter by mining, hauling, salvage, combat, or all<br>`query:<value>` — Optional mission title | — |
| `/mission mining` | Browse mission records related to mining, ore, and refinery gameplay | None | — |
| `/mission path` | Show the prerequisites, reputation, systems, and rewards for one mission | `mission:<value>` **required** — Select the mission whose unlock path you want to understand | — |

## note

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/note add` | Save a tip, route, workaround, procedure, or guide for this server | `title:<value>` **required** — Short searchable title for the note<br>`body:<value>` **required** — The useful information, instructions, warning, or workaround<br>`category:<value>` — Select an existing category or type a new one<br>`tags:<value>` — Optional comma-separated search words<br>`game_version:<value>` — Optional game version where this was confirmed, such as 4.9 LIVE<br>`source_url:<value>` — Optional reference link supporting the note | — |
| `/note categories` | List the community note categories currently used in this server | None | — |
| `/note delete` | Delete a suggested note you wrote or manage as a server administrator | `note_id:<value>` **required** — Select the community note you want to delete | — |
| `/note edit` | Edit a suggested note you wrote or manage as a server administrator | `note_id:<value>` **required** — Select the community note you want to edit<br>`title:<value>` — Replacement title; leave blank to keep the current title<br>`body:<value>` — Replacement note text; leave blank to keep the current text<br>`category:<value>` — Replacement category; leave blank to keep the current category<br>`tags:<value>` — Replacement comma-separated tags<br>`game_version:<value>` — Replacement confirmed game version<br>`source_url:<value>` — Replacement reference link | — |
| `/note list` | Browse recent community notes, optionally within one category | `category:<value>` — Optional category filter; suggestions come from this server<br>`limit:<value>` — How many notes to display, from 1 to 25 | — |
| `/note search` | Search this server's note titles, text, tags, and categories | `query:<value>` **required** — Words to find in note titles, text, tags, or categories<br>`category:<value>` — Optional category filter; suggestions come from this server | — |
| `/note verify` | Confirm that a suggested community note still works in the current patch | `note_id:<value>` **required** — Select the community note you personally confirmed | — |
| `/note view` | Open one suggested community note by its ID | `note_id:<value>` **required** — Select the community note you want to open | — |

## ops

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/ops add_job` | Add a gathering, hauling, or other job to your activity | `operation:<value>` **required** — Choose an activity you lead<br>`title:<value>` **required** — What needs to be done | — |
| `/ops create` | Create an activity and post a crew signup board | `title:<value>` **required** — A short name for the activity<br>`activity:<value>` — What you want to do together<br>`starts:<value>` — When to start: 30m, 2h, or a date with timezone<br>`meeting_point:<value>` — Where the crew should meet<br>`capacity:<value>` — Maximum crew size<br>`region:<value>` — Preferred server region<br>`ships:<value>` — Ships to bring, if any<br>`notes:<value>` — Anything the crew should know | — |
| `/ops from_craft` | Turn a crafting plan and its material shortages into a crew activity | `blueprint:<value>` **required** — Choose a crafting blueprint<br>`quantity:<value>` — How many finished items to make<br>`starts:<value>` — When to start, such as 30m or 2h<br>`meeting_point:<value>` — Where the crew should meet | — |
| `/ops job` | Claim, release, or complete a crew job | `operation:<value>` **required** — Choose an activity<br>`action:<value>` **required** — What to do with the job<br>`job:<value>` — Choose a job; omit to claim the next available one | — |
| `/ops join` | Join an activity or change your crew role | `operation:<value>` **required** — Choose an activity<br>`role:<value>` — Your role in the crew | — |
| `/ops leave` | Leave the crew and release your unfinished jobs | `operation:<value>` **required** — Choose the activity to leave | — |
| `/ops list` | Find activities and open crew slots in this server | `include_closed:<value>` — Also show completed and cancelled activities | — |
| `/ops materials` | Release reserved materials or record that they were consumed | `reservation:<value>` **required** — Choose a material reservation<br>`action:<value>` **required** — Release it, or deduct materials that were actually used | — |
| `/ops post` | Post or replace the signup board in this channel | `operation:<value>` **required** — An activity you lead or manage | — |
| `/ops remind` | Request or stop a personal DM reminder for an activity you joined | `operation:<value>` **required** — An upcoming activity you joined<br>`enabled:<value>` — Request a reminder, or turn it off<br>`minutes:<value>` — Minutes before the start; default 15 | — |
| `/ops reminders` | Review your activity reminders and any failed DM deliveries | None | — |
| `/ops reserve` | Set aside shared materials so another activity cannot use them | `operation:<value>` **required** — An activity you lead<br>`item:<value>` **required** — Shared inventory entry<br>`quantity:<value>` **required** — Amount to reserve from that entry | — |
| `/ops schedule` | Pause, resume, or remove a weekly schedule you own or manage | `schedule:<value>` **required** — Weekly schedule ID from /ops schedules<br>`action:<value>` **required** — Pause future boards, resume delivery, or remove the schedule | — |
| `/ops schedules` | Review weekly activities and board delivery problems in this server | None | — |
| `/ops show` | Open an activity, its crew, jobs, and material reservations | `operation:<value>` **required** — Choose an activity in this server | — |
| `/ops status` | Start, complete, or cancel an activity you lead | `operation:<value>` **required** — Choose an activity<br>`status:<value>` **required** — The new activity status | — |
| `/ops weekly` | Repeat an activity each week with a fresh crew board in this channel | `operation:<value>` **required** — An activity you lead to use as a template<br>`first:<value>` **required** — First local start: YYYY-MM-DD HH:MM, within seven days<br>`timezone:<value>` **required** — IANA zone such as America/Los_Angeles, Europe/London, or UTC | — |

## refinery

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/refinery best` | Compare refinery options for a resource by yield, speed, or cost | `resource:<value>` **required** — Resource you intend to refine<br>`priority:<value>` — How SCC should rank the options | — |
| `/refinery cancel` | Cancel a tracked refinery job and its reminder | `job:<value>` **required** — Choose the job to cancel | — |
| `/refinery collect` | Mark a refinery job as picked up | `job:<value>` **required** — Choose one of your completed refinery jobs | — |
| `/refinery jobs` | See refinery completion times and your pickup queue | `all_members:<value>` — Show the server’s jobs instead of only yours | — |
| `/refinery menu` | Open the connected SCC activity menu | None | — |
| `/refinery methods` | Browse refinery methods and their published yield, time, and cost values | `method:<value>` — Optional refinery method to prioritize in the results | — |
| `/refinery track` | Save a refinery job and optionally remind you when it is ready | `station:<value>` **required** — Where the refinery job is running<br>`material:<value>` **required** — What you are refining<br>`quantity:<value>` **required** — Cargo amount in SCU<br>`ready:<value>` **required** — Time remaining, such as 6h30m<br>`method:<value>` — Refining method chosen in game<br>`remind:<value>` — Post a reminder in this channel when the job is due | — |

## salvage

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/salvage plan` | Estimate salvage cargo trips and show current material sale options | `ship:<value>` **required** — Select the salvage ship or exact special variant<br>`material:<value>` **required** — Choose RMC or Construction Materials<br>`target_scu:<value>` **required** — How much material you intend to collect | — |
| `/salvage sell` | Find cached sale routes for RMC or Construction Materials | `material:<value>` **required** — Choose the salvage material to sell | — |
| `/salvage ships` | Browse ships and special variants identified for salvage gameplay | `ship:<value>` — Optional salvage ship or variant to inspect | — |

## ship

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/ship compare` | Compare two exact ships or variants, including acquisition and special-edition origin | `first:<value>` **required** — First exact ship or vehicle<br>`second:<value>` **required** — Second exact ship or vehicle | — |
| `/ship info` | Find an exact ship or vehicle, including special editions and acquisition locations | `name:<value>` **required** — Select an exact model or type part of a ship or ground-vehicle name | — |
| `/ship menu` | Open the connected SCC activity menu | None | — |
| `/ship shop` | List exact ships sold or rented at a dealership or rental terminal | `mode:<value>` **required** — Show purchases, rentals, or both<br>`location:<value>` **required** — Select a ship dealership or rental terminal | — |
| `/ship variants` | List standard, special, event, reward, and dealer variants in a ship family | `ship:<value>` **required** — Select any member of the ship family | — |

## status_watch

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/status_watch add` | Post official RSI outages and recoveries in a server channel | `channel:<value>` — Channel that should receive status changes; defaults to this channel | Manager |
| `/status_watch list` | List channels receiving official RSI status changes in this server | None | Manager |
| `/status_watch remove` | Stop official RSI status notifications in a server channel | `channel:<value>` — Subscribed channel to remove; defaults to this channel | Manager |

## support

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/support list` | Find open rescue and escort requests in this server | None | — |
| `/support post` | Post or replace your request board in this channel | `request:<value>` **required** — Choose a request you created or manage | — |
| `/support request` | Post a rescue or escort request with responder buttons | `kind:<value>` **required** — Rescue or escort<br>`location:<value>` **required** — Your location or meeting point<br>`details:<value>` **required** — What you need and what responders should know<br>`expires:<value>` — Time until expiry, such as 1h or 30m | — |
| `/support show` | Open a rescue or escort request and its controls | `request:<value>` **required** — Choose a rescue or escort request | — |
| `/support update` | Claim, release, arrive at, resolve, or cancel a support request | `request:<value>` **required** — Choose a rescue or escort request<br>`action:<value>` **required** — What to do with the request | — |

## trade

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/trade best` | Browse the highest-profit trade routes in SCC's current cache | `limit:<value>` — How many routes to display, from 1 to 15 | — |
| `/trade calculate` | Calculate cost, revenue, and profit for one exact cargo run | `commodity:<value>` **required** — Select or type the commodity being transported<br>`buy_terminal:<value>` **required** — Where you plan to buy; suggestions follow the selected commodity<br>`sell_terminal:<value>` **required** — Where you plan to sell; suggestions follow the selected commodity<br>`scu:<value>` **required** — How many SCU you want to carry | — |
| `/trade menu` | Open the connected SCC activity menu | None | — |
| `/trade plan` | Find profitable routes that fit your budget and ship capacity | `budget:<value>` **required** — Maximum aUEC available to buy cargo<br>`capacity_scu:<value>` — Usable cargo capacity in SCU; optional when you choose a ship<br>`ship:<value>` — Choose your ship to use its cached cargo capacity<br>`limit:<value>` — How many suggested routes to display, from 1 to 10<br>`system:<value>` — Optional system for both ends of the route, such as Stanton<br>`legal_only:<value>` — Only commodities marked legal by the provider<br>`max_age_hours:<value>` — Exclude unknown or older provider updates; optional<br>`container_size:<value>` — Only facilities supporting this container size; optional | — |
| `/trade routes` | Find profitable buy and sell routes for one commodity | `commodity:<value>` **required** — Select or type the commodity you want to haul<br>`limit:<value>` — How many matching routes to display, from 1 to 15 | — |

## trade_alert

| Command | Purpose | Options | Access notes |
| --- | --- | --- | --- |
| `/trade_alert add` | Notify a channel when a commodity reaches a profit-per-SCU target | `commodity:<value>` **required** — Select or type the commodity to monitor<br>`minimum_profit_per_scu:<value>` **required** — Minimum aUEC profit per SCU required before alerting<br>`channel:<value>` — Channel that should receive the alert; defaults to this channel | Manager |
| `/trade_alert list` | List commodity profit alerts configured for this server | None | Manager |
| `/trade_alert remove` | Remove one suggested commodity profit alert | `alert_id:<value>` **required** — Select the trade alert to remove | Manager |
