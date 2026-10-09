# Common questions

[Back to the docs](README.md)

## Where do I start?

Run `/start` and pick a task. **Crew** helps you join or plan a session; **Ships**, **Trade**, and **Crafting** are useful for browsing on your own. You don't need to learn the whole command list.

## Do I need a website?

Most features work in Discord. Optional Citizen iD linking opens a sign-in page. The bot owner's dashboard isn't needed to use SCC or manage it in your server.

## What does account linking do?

Citizen iD connects your verified RSI identity to the Discord account linked there. You can choose to show that RSI handle on crew boards. It doesn't link chat channels to the game, read your conversations, control gameplay, or automatically assign roles. `/lookup citizen` is a public profile lookup, not identity verification.

## Why is a ship price in Euros?

It's a real-money pledge price, shown separately from in-game aUEC. Choose USD, EUR, GBP, or hide pledge prices in **Settings**. If the source doesn't have your chosen currency, SCC labels the currency it does have.

## Can other people see my commands?

Choose public replies in **Settings** to share ordinary results. Identity, settings, reports, and reminders stay private. Crew and rescue boards are shared in their channel. This setting controls SCC's replies; Discord controls how the command itself is displayed.

## Can someone else use my menu?

Personal menus are yours, even when public. Others can open their own with `/start` or the shared hub. Crew and support boards have shared controls for eligible members.

## Why did my menu disappear or its buttons stop working?

Personal menus expire after ten minutes; `/help` expires after three. Run `/start` to open another. Use **Keep result** before it expires if you want to save the card without buttons. Shared hubs and crew or support boards stay available across restarts, but SCC needs to be online and have channel access.

## Can SCC find a player selling an item?

Yes. Look up a weapon or material with `/item`, or explore an ingredient from a recipe. Open **UEX marketplace** to search sellers or buyers and filter by price, quality, location, currency, and unit. Open the listing on UEX to contact the trader. Listings may be cached for five minutes, and reported stock and prices can change.

## Why are old menus still in the channel?

Current menus reuse their reply and clear when they expire. Older messages may still be there. **Close** removes a current menu; **Keep result** leaves the card. Shared hubs and crew or support boards are meant to stay.

## How often does the data update?

It depends on the source. Check the date and game version on a result; cached information may still appear during a provider outage. Use `/report_data` if something looks wrong. The bot owner can refresh sources with `/update`.

## Can SCC see my Discord status?

No. SCC doesn't monitor members' online, idle, or Do not disturb status. The owner can change SCC's own status and activity. Discord's [Streamer Mode](https://support.discord.com/hc/en-us/articles/218485407-Streamer-Mode-101) is a setting in your Discord app.

## Is everything translated?

Navigation, setup, reply choices, and command descriptions support ten languages. Some advanced forms and explanations still use English. Your personal language setting takes priority over the server's setting, with your Discord language used as a fallback.

## Where do my reports go?

`/bug`, `/suggest`, and `/report_data` go to the bot owner for review. They aren't automatically posted to GitHub. Before forwarding a report to a private repository, the owner reviews it and can remove sensitive details. GitHub issues you open yourself here are public.

## How do I remove my data?

Use `/identity unlink` to remove the saved account connection and display permissions. Revoking SCC in Citizen iD alone doesn't delete the connection already saved by SCC. For other access, correction, or removal requests, contact [AlphaTheWalf by email](mailto:AlphaTheWalf@gmail.com). Please keep private details out of public issues. See the [privacy policy](PRIVACY_POLICY.md).
