# Community activities

[Back to the docs](README.md)

## Plan a session

Open **Crew → Plan an activity** from `/start`. Enter a title, activity type, start time, meeting point, and crew capacity. You can use a relative start such as `30m` or `6h30m`; an absolute timestamp needs a timezone offset. The signup board appears in your channel, and Discord shows the start time in each member's local time.

Members can choose roles, claim jobs, and leave from the board. Leaders and managers control the activity's records and status. Use `/ops show` to open a saved activity or `/ops post` to repost its board. Completing or cancelling an activity releases unused reservations and closes crew actions.

## Run a weekly session

Use `/ops weekly` with an activity you lead. Enter the first local start as `YYYY-MM-DD HH:MM`, within the next seven days, and a timezone such as `America/Los_Angeles`, `Europe/London`, or `UTC`.

Each session gets a new board, crew signup, jobs, reservations, and earnings records. Boards are created up to seven days ahead. If SCC is offline during a session, it skips that missed session instead of posting it late.

Daylight-saving changes follow your chosen timezone. If a time occurs twice, SCC uses the first occurrence; if it doesn't exist, SCC moves forward to the next valid time.

Check `/ops schedules` to see upcoming sessions or delivery problems. Use `/ops schedule` to pause, resume, or remove a schedule you lead or manage. Removing a schedule stops future sessions but keeps activities already created. A server can have up to ten schedules and 100 open activities.

## Get a reminder

After joining a crew, click **Remind me** or use `/ops remind`. Choose a reminder from one minute to 24 hours before the start, and allow direct messages from the server. `/ops reminders` shows your requests and any delivery failures.

Leaving the crew cancels your reminder. Closed or expired activities don't keep sending reminders. For weekly sessions, request a reminder for each new activity. Delivery depends on SCC being online, your server membership, and your DM settings.

## Plan materials and split earnings

**Crafting** compares a blueprint's ingredients with your server's shared inventory. A plan doesn't reserve stock by itself. Leaders and managers can reserve materials with `/ops reserve`, then record what was used or released with `/ops materials`.

Saved plans keep the data from when they were created. Review any source-change warning, and use `/inventory verify` after checking the actual stock in game.

Members can claim and complete crew jobs from the board or `/ops job`. **Earnings** records income and costs, then calculates each crew member's share using their assigned weight. After paying someone in game, mark it with `/ledger paid`.

SCC doesn't read live game inventory, transfer aUEC, or confirm that a payment happened. Your group's records depend on what members enter.

## Show a verified RSI handle

You can participate with your Discord name alone. If you link a verified Citizen iD profile, use `/identity display` to let this server's boards show your RSI handle and last verification date. Display is off by default; earnings records keep Discord names.

Read the [privacy policy](PRIVACY_POLICY.md) for details about linked accounts and information already posted to boards.
