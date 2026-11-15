# MonoPbx nightly channel: what's new

## 1.0.0+20261115124700.1859804 (2026-11-14)

Live call triggers, custom statuses and a personal blocklist, chat retention with legal hold and export, executives with assistants, door phones, number porting, caller-ID names, an AI admin copilot and a simpler chat and Messages screen in MonoPhone.

### New

- **Live call triggers.** Admin, AI, Live call triggers: when a phrase or topic comes up on a live call, alert supervisors, post in chat, send a webhook event, add a CRM note, open a helpdesk ticket, tag the call or show a hint to the person on the call. Six ready-made triggers in nine languages are enabled with one click, and a tester shows what would fire on typed or spoken text. Never stores what was said; needs live assist with a speech provider.
- **Custom status.** Make a status of your own with a text of up to 60 characters, an emoji, a colour (available, away or busy) and an automatic end (30 minutes, 1 hour, 4 hours, today or this week). Colleagues see it in Team, in presence and in chat headers, and it can carry forwarding rules like any other status. In MonoPhone and the console.
- **Blocklist for calls and SMS.** Block or silence a number, a prefix or withheld numbers, for calls, SMS or both, optionally until a set time. A blocked caller hears rejected, busy or not in service; a silenced call goes straight to voicemail. Block from Recents or Contacts. Each user's list is their own.
- **Executives and assistants.** Admin, Calls and routing, Executives and assistants: an assistant screens the calls of an executive (outside callers only, or every caller), with a private line of numbers that always ring the executive. Assistants can set the executive's Do not disturb and forwarding when allowed.
- **Door phones.** Admin, Calls and routing, Door phones: SIP door stations ring people inside, show a still image of the camera and open the door with a key press in the call or a relay, also from the Open button in MonoPhone. An office-hours schedule decides when they ring.
- **Chat retention, legal hold and export.** Admin, Chat retention: a company retention period with the shortest and longest period a chat may set, and whether group owners and admins may set their own. Place a legal hold on a chat or a person (nothing is deleted while it lasts) and export a chat as PDF, JSON or ZIP with its attachments. Members see the period in force and any hold in the console and in MonoPhone.
- **Number porting.** Admin, Calls and routing, DIDs, Number porting: keep a port request in one place (numbers, account at the old carrier, the signed letter of authorisation, dates and carrier answers) with reminders. On the confirmed date the numbers join the chosen trunk by themselves.
- **Caller-ID names.** Admin, Calls and routing, DIDs, Caller names: the name each of your numbers shows on outgoing calls, and names for incoming outside callers looked up in the directory, company contacts and other sources.
- **Recording policies and card-payment pause.** Admin, Recording: policies per company, site, extension, user, queue, number or trunk, with never, on demand and a percentage of calls. Pausing for a card payment can also hide the keys pressed while the recording is paused.
- **Storage compliance.** Admin, Backups, Storage status: one page for the backup state, extra backup copies on other storage destinations with their own schedule and retention, write-once storage and legal hold, signed manifests that prove a backup is unchanged, and alerts when a backup fails or is late. Also in MonoPhone's admin status.
- **AI admin copilot.** AI, Admin copilot in the console, and Settings, Admin, Copilot in MonoPhone: configure and troubleshoot the PBX in plain language. It looks things up with your permissions, shows every change as a preview before you apply it, logs it in the audit log and undoes a whole change set in one step. Uses your company's own AI model.
- **PBX updates in MonoPhone.** Settings, Admin, PBX updates: the installed version, Check for updates, the What's new notes of every newer version, and Install update with progress, for administrators with the matching permission.
- **Rich chat notifications.** Chat notifications on iPhone, iPad, Mac and Android show the sender's name and photo and are grouped per chat. Notifications never carry the message text through the push service.
- **Better browser notifications.** Answer or decline a ringing call and reply to a chat message from the browser notification; one counted notification per chat and per SMS conversation; the sender's initials as the icon; admin alerts named by kind that open the right page. On iPhone and iPad, Safari shows how to add the web phone to the Home Screen.
- **Hours for one date.** Office-hours schedules can have different hours for a single date. In MonoPhone, changing Today's hours applies to today only by default.
- **Password reset by e-mail.** Admin, Users: Send password reset mails a single-use link valid for one day. Also in MonoPhone's admin user page.

### Improved

- **One kind of chat.** A chat is now a direct message or a group. A group has two plain settings: Who can post (everyone or only admins) and Who can join (invited people only, anyone can ask to join, or anyone in the company). New groups take a name, photo and description. One list with All, Unread, Groups and Direct filters, and error messages that say what went wrong where it happened.
- **New Messages screen in MonoPhone.** A lean header with only New and a menu, one search field, one row of small filters, Archived chats folded into one row at the top, Mark all as read, and a clear reason when team chat is not available.
- **Admin and Supervisor menus in MonoPhone.** Both sections now open a side menu from the menu button or an edge swipe, with grouped entries, badges for counts and Back to MonoPhone at the bottom. Tablets show the Supervisor menu as a side list.
- **Contact and call details in MonoPhone.** Actions are shown as tiles that wrap instead of being cut, list rows keep only the Call button and open the details on tap, colleague and contact details list recent calls with that person, and About shows the version with Check for updates on one tile. MonoPhone also works better with older PBX versions.
- **Finish setup box.** While setup steps remain, a box at the top of the admin home shows how many are left and continues with the next one. It can be collapsed, or hidden for the whole company.
- **Call flow editor.** A palette of components grouped by kind sits next to the canvas. Remove a node with its ×, the Delete key or Delete node (with a confirmation when it has connections, and undo), and a click on a node opens its properties.
- **Call pull is clearer.** Dialling `*85` when there is no call to pull now says "No call to pull" instead of reporting an unknown feature code, and MonoPhone shows the pull button only when one of your calls can be pulled.
- **Integrations page.** Admin, Integrations shows a searchable list next to the details of the selected integration: what it does, the data it reads and writes, its permissions and settings. The install form puts required fields first and masks stored secrets.
- **Single sign-on.** While single sign-on is required, accounts without a system role are given no password, and the sign-in pages say so. Accounts created on first sign-in get an extension from a range you choose, SAML group claims can also set the department, and identity providers with ECDSA keys are supported.
- **Sites.** A new phone joins its user's site, or the site whose network it is provisioned from. A site you choose by hand is kept.
- **Web phone ringing and closing.** Outgoing calls in the web phone play a ringback tone until answered (or the network's own tones), the ring volume can be set, and an × closes the phone. During a call it asks whether to keep the call in the background or hang up, and never hangs up by itself.
- **MonoPhone polish.** Opening the Admin section asks only for your passkey when you have one, with no separate password. Chat and SMS headers show the other person's photo or the group picture, Team shows a colleague's custom status emoji on their photo, and keypad tones moved to Advanced settings.
- **BI feed ready out of the box.** Admin, BI feed: the feed is set up by the installer and the updater, so you only create a BI user; no server settings to edit.
- **Toll-fraud limits per calling profile.** Calling profiles can set their own limit on simultaneous international calls and calls per hour at night.
- **Dialer campaigns.** A compliance page per campaign shows calling-window checks and the abandoned-call rate; contacts can be edited and imported from a file, and opt-outs imported from CSV.
- **API changes.** On chat message tasks the field `external_key` is now `external_ref`. Chat lists (mentions, starred messages, threads, the Shared tab, reactions, scheduled messages, reminders) are paged with `cursor` and `next_cursor`; the `before` and `before_seq` parameters were removed. Following threads, starring, chat settings, company chat controls, poll votes, scheduled messages and reminders now require `If-Match` when changed, and their answers carry a `version`. Update scripts and integrations that use these.

### Fixed

- SIP trace now captures calls made from MonoPhone and the web phone on installs where the console and the call engine run on separate servers; such traces showed no calls before.
- Install update in Admin, Updates showed the previous update as already installed and stopped; it now shows the progress of the new one at once.
- MonoPhone: Make default now switches the line, the keypad and outgoing calls to that account at once and is remembered at the next start. It is shown only when the phone has more than one account.
- Backups failed on installs updated to the version with sites; they run again.
- Profile photos uploaded from MonoPhone showed as broken images in the console.
- MonoPhone: call recordings and voicemail in the Admin and Supervisor sections now play on iPhone and Android, from the loudspeaker, and an error says exactly why a file cannot be played.
- MonoPhone: a phone set up with a setup code no longer asks for a password sign-in.

### Security

- Security fixes (low): sign-in and account protection, and data separation between companies.

## Earlier releases

### 1.0.0+20261115010156.3e51443 (2026-11-13)

SIP tracing in the console, chat channels and webhooks, a MonoPhone admin section, toll-fraud protection, storage destinations, live captions and calls that recover by themselves. After updating, calls to high-risk destinations and premium numbers are refused until an administrator allows them (see Toll-fraud protection).

#### New

- **SIP trace.** Admin, Logs, SIP trace: trace one extension, trunk or number, or a caller, called number or address, for a set time and with limits on calls, messages and size. Watch the messages live as a ladder diagram, open any message in full, search, and download a pcap file per call or for the whole trace.
- **Readable SIP events.** Admin, Logs, SIP events: each line opens into the request and every response. A sign-in challenge and its retry are shown as one line, and a reason code explains in plain words why a call failed. Links start a trace of the extension or the peer, or open the call. SIP events now also name the trunk.
- **Toll-fraud protection.** Admin, Call routing, Toll fraud and CLIR (Toll-fraud policy): built-in lists of high-risk destinations and premium numbers, your own blocked and allowed prefixes (or allow listed destinations only), a night-time limit, a limit on simultaneous international calls per user, and an automatic temporary block when international calls suddenly spike. Current blocks are listed there and can be lifted.
- **Action after updating: high-risk calls are refused.** Calls to the built-in high-risk destinations and premium numbers are refused until an administrator allows them in Admin, Call routing, Toll fraud and CLIR (Toll-fraud policy). Allow only the destinations your company really calls.
- **Chat announcement channels, webhooks and rich cards.** Announcement chats where only chat admins post (members can still react), chat admins and pinned messages, and webhooks per chat so other systems can post messages and rich message cards into a chat. In the console and in MonoPhone.
- **Chat: mute and delete.** Mute a chat for 8 hours, a week, until a chosen time or until you turn it back on, and still be notified when someone mentions you if you like. Delete a message for yourself or for everyone (within 48 hours; moderators at any time), or clear a chat for yourself.
- **Chat channels, groups and media.** Every company gets What's new, General and Announcements channels; What's new shows the release notes of each installed update. Create groups and channels with a description, picture and visibility; find, join or ask to join them; pin and archive chats. Send photos, videos, your location and voice notes, and share files through links that expire.
- **MonoPhone admin section.** Administrators can now manage the PBX from MonoPhone (Settings, Admin): users, phone setup, devices and who is online; live calls, office hours, forwarding, queues and IVR; system status with push alerts for administrators, company call history with the readable SIP view, and the audit log; voicemail and recordings; SMS, eSIM and licence (view only). Each screen appears only with the matching permission, and the server checks every action as it does for the console.
- **Passkeys in MonoPhone and confirmation for admin actions.** Sign in to MonoPhone with a passkey on iOS, macOS and Android, with the same passkeys as the console. Before opening the app's Admin section and before destructive admin actions, MonoPhone asks for a passkey, or the password and the second factor; a confirmation stays valid for ten minutes. Switch it in Admin, Security.
- **"That wasn't me" notices.** When a QR code, setup link or setup code is used to set up a device, the user and the administrator who issued it get an e-mail and a chat message from MonoPbx Security with the device, the approximate country, the address and the time. "That wasn't me" removes the device and ends its sign-ins at once.
- **Live captions.** Supervisors can turn on live captions for a queue call on the supervisor page, recognised on the server with the company's speech provider. Captions reach only the people on the call and the supervisors who joined, and an announcement tells the callers first. Rules in Admin, AI calls: consent, transcripts and verification codes; saving the captions as a transcript is off by default and has a retention period. Switch the feature on in the AI settings.
- **Storage destinations.** Send files to Amazon S3, S3-compatible storage, Google Cloud Storage or Azure Blob storage, for the whole install (Admin, System, Install storage destinations) or per company (Admin, Storage destinations). Encryption options, write-only credentials, and a Test connection button that names any missing permission. Every upload is checked after it is written, and the local copy is released only then.
- **App update checker.** MonoPhone tells you when a newer version is available in the App Store or Google Play, and the PBX can set a minimum and a recommended app version. About now shows the real app version.
- **Siri, Shortcuts and Live Activity on iPhone.** Ask Siri or use Shortcuts to call a colleague or a number, set your status or hear who is on a call. During a call, the Lock Screen and Dynamic Island offer Mute and Hang up and show "Reconnecting…" while the call recovers.
- **Ongoing-call card on Android.** The call notification shows the timer (also on hold), "Reconnecting…" while the call recovers and a Mute button that works on the lock screen. Calls can be added to the phone's call log, and Bluetooth, car audio and holding for a mobile call go through the system.
- **Second-factor banner.** The console shows a red banner while your account has no second factor (an authenticator app or a passkey), with a link to set one up.
- **What's new in the console.** Admin, Updates now shows the release notes of every version newer than the one installed, next to the Update button and in the confirmation, and shows what changed right after an update.
- **Default speech model per AI provider.** In Admin, AI, Providers you can set the speech-to-text model a provider uses by default and see which kind of credential it holds. A model chosen on a feature still takes precedence.
- **Profile photos in MonoPhone.** Change your own photo in MonoPhone (Settings, My profile: take a photo or choose one, then crop it). Colleagues' photos now appear in Contacts, Recents, call screens, voicemail, Messages and Chat.
- **Reconnecting during calls.** When a phone's connection drops for a moment, MonoPhone shows "Reconnecting…" in place of the call timer and restores the audio by itself; the timer continues where it was. The PBX also notices when one side of a call stops sending audio and asks the app to reconnect.
- **Chat collaboration.** In the console and in MonoPhone: react with any emoji and see who reacted; reply in threads and follow them; mention `@all` or `@here` where the chat allows it, and find your mentions in one list; sent, delivered and read ticks with "Seen by"; forward messages to up to 10 chats; link previews; start a group voice or video call from a chat and join a running one; a Shared tab with the media, files, voice notes and links of a chat; saved messages; and polls.
- **Chat: plan, prioritise and get help.** Send a message later and set reminders; mark a message as urgent; summarise, translate and draft replies with AI (always labelled); create a task in a connected system from a message; and set your own quiet hours and out-of-office answer.
- **Chat controls.** Admin, Messaging, Channels, Chat controls: set company rules for read receipts, link previews, urgent messages and who may mention everyone.
- **Sites.** Admin, People, Sites: group departments, users, devices, trunks and numbers into sites, each with its own country, time zone, address and music on hold. Outbound rules can apply to chosen sites, and a site's local trunk is used first for its calls (local breakout). Site reports with export, and site administrators who manage only the departments of their site.
- **Call costs, account codes and spend limits.** Admin, Call routing, Call costs: set rates per trunk (connection fee, minimum, billing increment) and see what answered outgoing calls cost, by user, department, cost centre, site, code or trunk, with a chargeback export. Require a project or authorisation code for chosen kinds of destination (on desk phones dial `*55`, the code, `*` and the number; MonoPhone and the web phone ask for it). Daily or monthly limits on cost or minutes for the company, a department, a site or a user warn first and then block calls or ask for an authorisation code.
- **Setup guide.** Admin, System, Setup guide: after the first-run setup, a guided list of steps with progress, the time left, Skip for now and a Test button that explains how to fix a problem. Steps 1 to 4 are guided in place: licence or trial, company and region (country, time zone, language, currency, number format), your domain with a DNS check, and office hours with the public holidays of 20 countries. The dashboard shows a "Finish setting up" card until you are done.
- **Live captions in MonoPhone.** Turn on captions during a call: recognised on the phone by default (nothing leaves the phone), or by the company's speech provider when that feature is on. Choose the language, copy the captions or save them to the call's notes when the company allows it.
- **iCloud in MonoPhone.** iPhone, iPad and Mac offer to save your sign-in to iCloud Keychain and fill it in on your other devices; the list of PBX addresses, the appearance and keypad tones sync through iCloud; voicemail and team recordings can be saved to Files or shared.
- **Focus and Contacts on iPhone.** Focus filters set your MonoPhone status (for example Do not disturb) while a Focus is on and restore it afterwards. Colleagues can be added to the iPhone's Contacts in their own group, with photos (off by default; removed again when you turn it off or sign out).
- **Widgets and Watch.** A new Admin widget on iPhone (Home and Lock Screen, StandBy) and a Night mode widget on Android show night mode of your office-hours schedules and who is on a call, for administrators with the matching permission. A new Presence complication on Apple Watch stays current while the watch app is closed. Android widgets use the phone's Material You colours.
- **Android chat notifications, sharing and saved passwords.** Chat messages appear as conversations with the sender's photo, Reply and Mark as read, and as bubbles for direct and pinned chats. Recent chats appear in the share sheet, so you can share text, photos, videos and files into a chat. MonoPhone can use and save passwords from the phone's password manager, and offers your PBX addresses again after you reinstall or move to a new phone.
- **Move a call between iPhone, Apple Watch and Mac.** Move a running call to another of your devices, or tap "Take it here" on the device you want, without the caller hearing a ring or hold. Handoff continues calls, chats and contacts on your other Apple devices, and on iPhone you can share photos, files and links into a chat from any app.
- **Managed Android phones.** Mobile device management can set MonoPhone's server address (and lock it), the sign-in e-mail or domain, require a passkey and turn off the device contacts book.
- **SIP trace with audio.** Admin, Logs, SIP trace: a trace can also capture the call audio, with limits per call and per trace, and the pcap files then carry the audio next to the SIP messages (where the install stores recordings). Refused registrations and messages now carry a reason code in SIP events too.

#### Improved

- **Contacts and Recents in MonoPhone.** A Message button on each colleague opens the chat, contacts have a Text action when SMS is set up, and Recents shows full numbers and opens call details (call, video, message or text, add to contacts, favourite, copy). MonoPhone also shows a microphone level during calls and plays audio clips inside inbox messages.
- **Single sign-on and SCIM.** A new Sign-in policy in Admin, Single sign-on can require single sign-on for the company (a break-glass administrator sign-in is kept and you cannot lock yourself out) and create accounts on first sign-in with a department, role and licence limit. A directory group can be mapped to administer one department; adding or removing a mapping now updates current members at once, SAML group claims can grant roles, and API keys of a removed user are revoked. Departments now lists each department's administrators.
- **Invitation links last 7 days.** App setup links, setup codes and user invitations are valid for 7 days by default. Change it from 1 to 30 days in Admin, Security, Invitation links; links already sent keep their expiry.
- **The administrator always has an extension.** Setup now always creates the administrator's extension, with a voicemail box and a MonoPhone device, and the last setup step shows the MonoPhone QR code. After updating, every System Owner without an extension gets one.
- **Faster console.** The console loads about a third less code when it opens, so the first page appears sooner.
- **Supervisor monitoring stays silent.** Listening, whispering and barging in stay silent by default; a beep for the agent or for everyone remains a choice in the supervisor settings.
- **Calls recover after a media restart.** Conferences, calls answered by apps and calls the PBX placed are restored after a media service restart, and a recorded conference continues recording as a new part. Problems of the media service now appear in the system log.
- **Integrations.** WhatsApp calling as a trunk type in the trunk form; Jira: Sync now, the last sync result and SLA rules per destination; a Notion page picker and clearer field errors; opt-outs kept in step with connected marketing tools; delivery orders in the inbox; icons and descriptions in the integrations catalogue; a yes-reply on WhatsApp accepts a queue callback offer; public holidays for more countries and the company time zone in the dialer.
- **API changes.** Fields were renamed: AI provider `credential_kind` is now `auth_kind`, chat webhook `secret_hint` is now `address_hint`, integrations `secrets_set` is now `filled_settings`, and the Jira SLA `key` is now `issue`. The chat user mapping list is now paged with `next_cursor`. Several chat, hotel and settings changes now require `If-Match`. Update scripts and integrations that use these.
- **Admin menu.** Sidebar sections start collapsed and remember which ones you opened, per browser. The section of the page you are on still opens by itself.
- **SMS centre address.** The SMS centre address of the mobile core (Admin, IMS) now defaults to `123`, so eSIM orders and SMS work without setting it first. An address you already set is kept.
- **Sessions and sign-ins in MonoPhone.** Active sessions and new sign-in alerts are now one page; pull down to refresh. A phone set up from the app setup page is listed under its app name instead of the browser's name.
- **App setup links.** The app setup page checks the link first and explains when it has expired, was already used or was replaced by a newer one, instead of opening the app with a link that cannot work.
- **Built-in mail service.** Installs on a trial can send as many e-mails through the built-in mail service as licensed installs. When the sending limit is reached, the console says so and links to Admin, E-mail to set up your own provider.
- **Licence changes apply faster.** Changes to your licence apply within about a minute, without a restart. With its licence check-in the PBX now also sends a short technical health summary (counts, service status, certificate expiry dates, load); it contains no call, message or contact data.
- **AI receptionist templates.** When a template creates an opening-hours schedule, the agent's after-hours greeting now follows that schedule automatically.
- **Leave-a-voicemail code is now `*88`.** Dialling `*88*` and an extension leaves a voicemail directly (was `*84`), so the code no longer clashes with call-park slots. Companies that never changed their dial codes move automatically; a code you changed yourself is kept. Tell your users if they used `*84`.
- **Licence checkout.** Buying or changing a licence shows the current plans, add-ons and prices for your country and currency, accepts coupon codes, and add-ons assigned to you now raise your licence limits.
- **Privacy requests include live captions.** A person's privacy export and erasure now cover saved live-caption transcripts.
- **Setup guide API.** In the setup guide steps the field `key` is now `step`, and changing a step or hiding the guide requires `If-Match`.

#### Fixed

- MonoPhone: pasting into the dialer number field works on iOS, Android and macOS. An empty dialer offers "Paste number", and pasted text is cleaned up (spaces, dashes, brackets, call prefixes, other digit styles, an extension); text that is not a number is refused with a hint.
- MonoPhone: tapping a setup link while the app was closed opened the sign-in screen and did nothing; it now signs in.
- Messages taken by an AI agent now light the message-waiting lamp on desk phones and count as unread, also for users without a voicemail box.
- An expired or signed-out session no longer counts towards the automatic blocking of an address after failed sign-ins.
- A call that ends unexpectedly now disappears at once from the switchboard of department-limited users.
- Calls that were picked up again after a server restart can be put on hold with music on hold.
- The limit of callback requests per caller number now also holds when several requests arrive at the same moment.
- One side of a call could lose audio on mobile data while the call stayed up; such calls now recover. A quiet media server is no longer mistaken for a restarted one after the last call ends.
- AI events sent to webhooks (handover, outbound calls, low answer rate) are no longer lost when the server restarts at the wrong moment.
- Queue views no longer keep showing agents who were deleted or removed from a queue.
- The button on the app setup page could become unreadable on iPhone after tapping it.
- MonoPhone: long filter labels no longer overflow their buttons, and the call status line fits small phones and long calls.
- Kubernetes installs with a separate SIP engine: the engine's monitoring port no longer clashes with the media service, and the SIP engine can use an external database.
- MonoPhone on Android: a second incoming call could be answered by mistake when the first call was answered on the notification; it now rings on its own.
- Simultaneous changes to hotel rooms and guests no longer overwrite each other.
- Deleting a company now also deletes its SIP events right away.

#### Security

- Security fixes (medium): connecting and disconnecting an online store integration is checked more strictly, and disconnecting now also revokes the PBX's access at the store.
- Security fixes (medium): connections to company storage destinations are checked more strictly.

---

Latest build: `1.0.0+20261115124700.1859804` (commit `1859804`), published 2026-11-15T13:30:57Z.

Images (by digest):

- MPBX_IMAGE=ghcr.io/ilinaya/monopbx@sha256:ab79044dccb3101e6d1ba51d8ff6605eea1a59bfd0c5f14a5e3666eb19f466f4
- MPBX_RTPENGINE_IMAGE=ghcr.io/ilinaya/monopbx-rtpengine@sha256:d3282e303dee15992979beef993cb36bcdc5be709691743faa603d610a4da7c7
- MPBX_MEDIA_IMAGE=ghcr.io/ilinaya/monopbx-media@sha256:32ec9c96b36cffc652394b76e795f5bc474c2dd6ce0cf7acc145899e0bd60c24
- MPBX_UPDATER_IMAGE=ghcr.io/ilinaya/monopbx-updater@sha256:04e4b45697608afb9dbd72f0d9fb86313f0021e820a07cc8572fdefcbaf52b35

A build installs over any older build of the same major version. Check for updates in the console (Admin, Updates).
