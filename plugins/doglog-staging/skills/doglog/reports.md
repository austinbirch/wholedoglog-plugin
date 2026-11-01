# Questions and reports

Read from the skill when the owner asks how the dog has been, about a
pattern or a change, for the dashboard, or for outside data such as weather.

- doglog is the record. Don't make or offer a spreadsheet, document, file
  or artifact of it, or keep a copy elsewhere: a second copy goes stale and
  splits the diary. Show things with doglog's blocks and views, or in a few
  lines of chat where they can't yet.
- Look things up with `query_facts`, reading the dumps for anything no
  tracker holds.
- Show, don't list. doglog is one app made of pieces you put together
  in the conversation, each in its own look; answer with them and a line
  or two of your own, never the same thing as bullets.
  - The built-ins, the same every time, for the questions every owner
    asks: review (a day, "show me today"), days ("how's his week been?"),
    month ("how was October?"), overview (the front of their diary, "open
    his diary"), watching (what you watch for them), log (what they said,
    day by day), and the dashboard (`get_view`, below).
  - The pieces, which you shape to the question with `render_block`: stat
    (where something is and which way it's going), series (over time, up
    to five marks from the record, meds changes by default; over months
    `by: "week"` or `"month"`), compare (periods side by side, before and
    since a change), notes (their words on a topic, quoted exactly),
    callout (one thing said big: how many good or harder days in a range,
    a tracker since a change against as long before, a run of days, on how
    many days a yes/no, count or choice happened, or how long since it last
    did: "sick on 2 of the last 7 days", "12 days without"). A series draws
    weight and counts too, with their units, and a choice whose options run
    best to worst.
  - Several in one reply when you're walking through it: a card, a line of
    yours, the next card ("here's October… and here's his sleep across
    it"). Built-ins and pieces mix freely.
  - One card with `show` when it's a single answer to take in at once
    ("how has he been since the dose change?"): blocks in the order you'd
    explain them, two stats as a `pair`, and a heading or a line of your
    own between them, never a number of your own.
- For "is X doing anything?", compare the tracker they care about before
  and since X, in days and plain averages. Then say what else changed meanwhile
  (meds, supplements, food, weather, routine), so the answer claims no
  more than the facts do.
- Answer the question asked, even when the answer is no. Say what the data
  can't see rather than stretch it. A weaker pattern is worth raising with
  its size, its number of days and what else changed then. No correlation
  coefficients or formulas, ever.
- Every dog has a dashboard, the picture to come back to: `get_view` for
  "how's he doing?", opening full screen from the card. Until shaped it's
  what's watched, overall score first. Change it with `save_view`, sending
  every block in order (the overall score stays on top); `reset` restores
  it. `get_view` also gives its link, a page needing no sign-in: give it
  when they want the dashboard outside the chat, and say anyone with it can
  see it. If it's gone further than they meant, `replace_dashboard_link`. Other
  saved views, and a link for the vet, aren't there yet.

## Outside data

Fetch outside series (weather first) with `backfill`, only when asked or
when they've agreed to keep it coming, for the days there are facts for. It
needs the dog's location: ask where in plain words ("a town or village is
plenty"), turn it into coordinates yourself, and save it with `setup_dog`.
doglog doesn't look places up.
