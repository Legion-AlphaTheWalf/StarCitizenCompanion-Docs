# Getting started

[Back to the docs](README.md)

## Open SCC

Run `/start` in your server, or click **Open my SCC panel** on a shared hub. On your first visit, choose your language, pledge currency, ship budget, and private or public replies. Select **Save and open SCC**, or **Use SCC now** to keep the defaults.

Setup and the menu it opens are private. Your reply preference applies to later searches and visits. You can change it any time in **Settings** or `/settings`.

## Pick something to do

| Section | What you can do |
| --- | --- |
| Home | Get help or read the latest updates |
| Crew | Find a crew, plan an activity, or request rescue and escort |
| Trade | Find a run for your budget and cargo space; track a refinery job |
| Ships | Search for a ship or browse by role and budget |
| Crafting | Look up items and blueprints, explore ingredients, or check shared inventory |
| Mining | Look up resources and equipment, plan a trip, or compare refining options |
| More | Check mission requirements, share notes, look up RSI profiles, or link your account |
| Settings | Change your preferences |

The section you're viewing is highlighted in blue. Some features may be disabled by your server's managers.

You can also open a topic directly with `/trade menu`, `/mining menu`, `/craft menu`, or `/ship menu`. Use the topic buttons or **Go to another activity** to move between them.

## Items, recipes, and source links

Try `/item query:Karna Rifle` to see a matching recipe, shops, and sources. `/blueprint query:Karna Rifle` takes you straight to the recipe. Run either command without a name to open Crafting.

When viewing a recipe:

- Select an ingredient under **Explore an ingredient or related result** to look it up in SCC. Use **Back** to return.
- Open **Wiki page** or **Wiki search** to read more in your browser.
- Choose **Plan materials** to compare the recipe with your server's shared inventory, or **Source materials** for gathering guidance.
- Use **Next details** and **More related** when a recipe has more information than fits on one page.

You'll also find source links in ship, trade, mining, refinery, mission, salvage, location, and public RSI results. **Wiki data record** opens the original data behind a result. Wiki search links are used when SCC doesn't have a direct article link.

If SCC can't find a recipe or price, that doesn't mean the item is unavailable in game. Wikelo barter rewards are shown separately from crafting recipes. Blueprint browsing works in DMs; shared inventory planning needs a server.

## Find a player seller or buyer

Weapon and material results can suggest UEX player sellers. Open **UEX marketplace** to browse **Find sellers** or **Find buyers**. You can filter by price, quality, and location.

Select the currency and unit before comparing prices. SCU, cSCU, boxes, and individual items are listed separately; SCC doesn't convert between them. Quality uses UEX's 0–1000 scale. Listings with unknown quality are excluded when you set a minimum.

Player listings are separate from NPC shop prices. They refresh on demand and may be cached for up to five minutes. If UEX is unavailable, a recent cached listing may appear with a warning. Prices, stock, and availability come from traders and may have changed.

Open the UEX listing to contact a seller or buyer. SCC doesn't place orders, publish listings, or send messages to traders. You don't need a UEX account key to browse.

## Keep the channel tidy

Searches and topic changes usually update the same menu. **Close** removes it. **Keep result** leaves the card without buttons and keeps its existing privacy setting.

Unused personal menus clear after ten minutes; `/help` clears after three. Open `/start` again to continue. Shared hubs and crew or support boards stay in place. Cards you choose to keep also remain. Some older messages may still be in the channel.

Read **Home → What’s new** or the [changelog](CHANGELOG.md) for recent changes.

## Private or public replies

**Private** replies are visible only to you. **Public** replies can be read by anyone with access to the channel. Even when public, your personal menu can only be used by you; others can open their own.

Account linking, settings, reports, reminders, subscriptions, and sensitive controls stay private. Crew and rescue boards are shared in their channel so other members can join. Reply preferences change SCC's responses, not how Discord displays the command you entered.

Your personal settings apply across servers. Choose **Use default** to follow a server's settings. Language falls back to your Discord language when no preference is set. Some advanced forms and explanations still use English.

## Prices and ship budgets

- In-game purchase and rental prices use **aUEC**.
- Real-money pledge prices are separate. Choose USD, EUR, GBP, or hide them. If a source doesn't have your currency, SCC labels the original currency; it doesn't calculate an exchange rate.
- Ship budget filters use available purchase quotes. Set it to zero for any budget. Searching for a ship by name ignores the budget so you can still view it.

Check the date and game version shown before buying or trading. Update times vary by source, and a listed price doesn't guarantee current stock. SCC doesn't transfer currency.

## Join a crew

Open **Crew → Find a crew**, choose an activity, and pick a role. Check the board for jobs and use **Remind me** if you'd like a private reminder. Leaving the crew cancels it. See [Community activities](COMMUNITY_ACTIVITIES.md) for planning your own session.

## Link your RSI identity, if you want

SCC works without account linking. Citizen iD verifies your RSI identity and matches it to the Discord account you've linked there.

Open **More → RSI linking** or `/identity link`, then finish signing in on the account page. `/identity status` shows the saved result privately. It reflects your last sign-in, so it isn't a continuous identity check.

To show your verified RSI handle on this server's boards, use `/identity display enabled:true`. Display is off by default and set separately for each server. Use `enabled:false` to hide it, or `/identity unlink` to remove the connection. Read the [privacy policy](PRIVACY_POLICY.md) for details.

Everyday features work inside Discord. Account linking opens a sign-in page; the bot owner's dashboard is separate.
