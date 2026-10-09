# Privacy policy

Last updated: October 8, 2026

## 1. Introduction and scope

I'm **AlphaTheWalf**, and I run the Star Citizen Companion Bot (“SCC” or “the Bot”). This policy explains what SCC stores, how I use and protect that information, and how to contact me about your data. By using the Bot, you consent to the practices described in this Privacy Policy.

## 2. Data collected and why

SCC stores the information needed for the features you use:

| Data | Purpose |
| --- | --- |
| Discord user/server/channel/message IDs and display names | Identify record owners and crew, enforce server isolation/permissions, deliver requested reminders, and update posted boards |
| Activities, crew roles, jobs, weekly templates, reminder requests/delivery state, refinery jobs, support requests, material reservations/history, and in-game earnings/payment records | Save community workflows across sessions and restarts |
| Inventory, blueprint ownership, debriefs, notes, and their author/verifier IDs and submitted text | Shared planning, record history and community references |
| Personal/server preferences | Language, pledge currency, ship budget, result visibility, feature switches and other settings |
| Bug reports, suggestions and data corrections, including reporter ID, display name and submitted text | My review, troubleshooting and requested improvements |
| Command-usage records: interaction ID, server ID, command path, locale, time, success/failure and error type | Operational counts and reliability monitoring. This analytics table omits user IDs, command arguments and message content |
| Technical logs and signed website session cookies | Diagnose service failures and support sign-in, authorization state and form protection |

SCC does not scan/store general channel conversations or monitor members' online/idle/DND status. Information deliberately submitted in a command/form may contain personal details; avoid putting passwords, financial details or other unnecessary private information into it. Game earnings are aUEC records, not bank/payment-card information.

### Optional Citizen iD connection

If you choose to link, SCC saves the identity provider/issuer, provider account identifier, Discord account ID, RSI handle, citizen ID, verification result and last linking/sign-in time. It uses the authorized profile/role claims to establish that saved result; it does not keep the full claims or role list as an identity record. Production and staging records are separate.

SCC does not save your Citizen iD password, email address, or OAuth access/refresh/identity tokens as stored account records. Verification reflects the last sign-in and may change later. Linking is optional; ordinary crew/trade features work without it. Optional Discord sign-in to my private dashboard uses the account ID to confirm it's me; it doesn't give members access to that dashboard.

## 3. Visibility, storage and retention

I store records in SCC's local database and protected backups; technical logs rotate. My private dashboard is restricted to me. Server-scoped records belong to that server, while personal preferences and linked-account records belong to the member.

Ordinary query replies are private by default, but server defaults and personal preferences can make them public. A public result and shared activity/support board can be seen by people with channel access. Sensitive identity/settings/report/reminder/control replies remain private. These reply settings do not make shared server inventory, notes or crew records confidential to their author.

Your verified RSI handle is hidden from crew boards until you enable display for that server. Enabled boards can show the handle and last verification date, as can the activity page on my private dashboard. Turn display off, use the account page's hide-everywhere control, or unlink to revoke that display permission. SCC queues updates to tracked boards and retries failed edits a limited number of times. It cannot delete other people's copied messages/screenshots or guarantee removal from old untracked posts.

Operational records and reports can persist until removed through the available controls or handled by me; there is no automatic deletion deadline for every record. Inventory removal can leave audit/history records. Command analytics older than 180 days are pruned periodically. Logs rotate by file size rather than an exact number of days.

Full recovery archives are encrypted before transfer to my off-device backup storage. The local archive job retains the latest 30 archives; the off-device collector removes archives older than 90 days while retaining its latest copy. Protected local database/update snapshots and manually retained recovery copies can also exist. Backups may retain records removed from the active database until those copies are rotated or removed; unlinking is not an immediate purge of all historical backups.

## 4. Third-party services and sharing

- **Discord** carries bot interactions, public/private replies, boards and member-requested reminders, under Discord's own policies.
- **UEX, Star Citizen Wiki and StarCitizen-API** supply market/reference/public RSI data. A requested public citizen/org/system lookup can send that query to its provider; some results come from SCC's cache. Exact item/material marketplace lookups send the item name or identifier to UEX. SCC displays publicly advertised seller/buyer handles, listing details and links, cached in memory; it does not send Discord member identities to UEX for these searches. SCC does not send its stored crew, inventory or linked Citizen iD records to those market/reference providers as part of ordinary lookups.
- **Citizen iD** handles optional identity authorization/sign-in and provides the authorized identity claims under its own policies.
- **GitHub** hosts these public docs/issues. Bot reports are saved locally first. I can review and edit a redacted copy before choosing to forward it to a private repository. Redaction is not a guarantee that every private detail in free text will be detected. An issue you submit yourself in this docs repository is public.
- Website hosting/reverse-proxy/tunnel services carry requests to the account site and my private dashboard and can process technical connection information under their own policies.

I don't sell your data or share it with third parties for marketing purposes. Relevant provider resources: [Discord privacy](https://discord.com/privacy), [UEX](https://uexcorp.space/api/documentation/), [Star Citizen Wiki API](https://api.star-citizen.wiki/), [StarCitizen-API](https://v2.starcitizen-api.com/), [Citizen iD](https://citizenid.space/), and [GitHub privacy](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## 5. Data security

I use reasonable technical and organizational measures to protect your data from unauthorized access, disclosure, or alteration. However, no method of transmission or storage is completely secure, and I cannot guarantee absolute security. The hosted account site uses HTTPS, signed secure session cookies and form protection. Configuration and backup access are restricted. Keep private information out of public reports.

## 6. Access, correction and removal

You can contact me to request access to, correction of, or removal of your stored data. I'll need to verify your identity or ownership before handling the request. I'll respond within a reasonable timeframe, subject to applicable obligations. Depending on your jurisdiction, you may have additional rights; contact me for assistance.

Use `/identity unlink` or the account-page unlink control to remove your active saved connection and display permissions. You can also revoke SCC in Citizen iD; revocation there alone does not delete SCC's existing snapshot. Unlinking does not remove separate community records, copies already posted, or historical backups. Contact me about other records. No general automated member data-export/deletion command is currently available.

Managers can use `/analytics set enabled:false` to stop future command-usage recording in their server; older entries remain until pruning/removal. Members can cancel activity reminders or leave the crew to stop those reminders. Reminder preferences do not carry over to new weekly activities.

## 7. Changes to this policy

I may update this policy to reflect changed practices or legal requirements. I'll communicate significant changes through the Bot or related communication channels. Your continued use after changes indicates acceptance of the revised policy.

## 8. Contact

For questions or data requests, contact me (**AlphaTheWalf**) in Discord or [by email](mailto:AlphaTheWalf@gmail.com). Send requests privately, not through a public GitHub issue. See [security reporting](SECURITY.md).
