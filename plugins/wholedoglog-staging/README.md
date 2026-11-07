> **This is the staging build**, for testing a branch before it is merged. Its connector goes to the staging server, which keeps a copy of the record, not the real one. For a real dog, use the WholeDogLog plugin.

# WholeDogLog

A carer for your dog's health record, inside Claude. Tell Claude how your dog's
day went, in your own words, in any chat. Claude keeps the diary: it remembers
what was going on last week, checks in on the things you said you care about,
notices what you didn't ask it to watch, and answers questions about the
history with charts in the conversation.

WholeDogLog is a diary that makes vet conversations easier. It is not a vet and it
never diagnoses.

## Use it

Add this plugin from Claude's Customize > Plugins (or, in Claude Code,
`/plugin install wholedoglog --marketplace austinbirch/wholedoglog-plugin`), then add WholeDogLog from the plugin's Connectors tab. WholeDogLog asks for your email
and sends a six-digit code to type on the same page; there's no password.
Then just talk:
"Murphy was stiff this morning but ate well", "how has his sleep been this
month?", or "check in with me about Murphy". To be asked every evening,
create a scheduled task in Claude that says so.

If the sign-in ever lapses, Claude shows a Connect button in the chat to sign
in again. If anything is missing, Claude says so and walks you through it.

## What's in it

- **A skill**, `/wholedoglog`: how Claude keeps the diary, checks in, and reports.
- **A connector** to WholeDogLog's server at `wholedoglog.com`, which
  stores the record.

## Data

What you tell Claude about your dog, in your words, and what Claude records
from it (scores, notes, the things it watches) go to WholeDogLog's server, under
the email you signed in with, with any photos you upload and roughly where home
is, for the weather. WholeDogLog never runs an AI model of its own and
sees nothing from your chats except what Claude sends to its tools. The cards
WholeDogLog shows in the chat send usage, errors and masked session replays to
PostHog. You can download everything or delete your account at any time.

The full list of what's kept, who handles it and for how long is in the
[privacy policy](https://wholedoglog.com/privacy). Terms are at
[wholedoglog.com/terms](https://wholedoglog.com/terms), and help at
[wholedoglog.com/help](https://wholedoglog.com/help).

## Support

Write to support@wholedoglog.com.
