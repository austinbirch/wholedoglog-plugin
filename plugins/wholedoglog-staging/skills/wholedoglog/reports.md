# Questions and reports

Read from the skill when the owner asks how the dog has been, about a
pattern or a change, for the dashboard, or for outside data such as weather.

- WholeDogLog is the record. Don't make or offer a spreadsheet, document, file
  or artifact of it, or keep a copy elsewhere: a second copy goes stale and
  splits the diary. The one exception is the owner's own Google Sheet,
  kept up to date because they asked (`sheets`, in `setup.md`). Show things with WholeDogLog's blocks and views, or in a few
  lines of chat where they can't yet.
- Look things up with `query_facts`, reading the dumps for anything no
  tracker holds.
- Show, don't list. WholeDogLog is one app made of pieces you put together
  in the conversation, each in its own look; answer with them and a line
  or two of your own, never the same thing as bullets.
  A longer answer weaves your words and cards together: a short paragraph
  making a point, the card that shows it, the next point, its card. Where
  it stands (a stat or a callout), what happened lately (notes, by day),
  what's worth raising with the vet (a callout, or notes on that topic).
  Your words carry the reasoning and the caveats; the cards carry the
  numbers and the owner's own words. A wall of text after one card says
  the card twice and buries the points it could have shown.
  - The built-ins, the same every time, for the questions every owner
    asks: review (a day's report card, "show me today" or "how was yesterday?"), days ("how's his week been?"),
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
- The numbers you say are the card's. Every `render_block` and `show`
  result says the card's numbers in words: use those, the way the card
  puts them ("on 6 of the 12 days recorded"), and never count the dumps or
  facts yourself for something a card shows. Two counts of the same thing
  that disagree tell the owner something false about their dog. If you
  need a number no card gives, show the card that gives it. Write dates
  the way the cards do ("22 Oct", "Wed 22 Oct"), never "22/10".
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

Weather comes from `get_weather`: the daily rain, highs and lows, humidity
and pressure for any days, each at wherever they were that day (home, or
that day's place fact). Each day is kept as it's recorded, so reading is
quick. It needs a home. If `get_household` has none, ask where they live in
plain words ("a town or village is plenty"), turn it into coordinates
yourself, and save it with `setup_dog`'s `location`; WholeDogLog doesn't look
places up. Home is the household's, for every day; a day somewhere else is a
place fact on that day, corrected like any other.

- For "does the weather affect him?", `get_weather` for the days there are
  facts for, then compare the tracker they care about on wet and dry days (or cold
  and mild) in plain averages and day counts, using the days the result
  lists. Say how many days each side has, what else changed in those weeks,
  and what the record can't see (whole days, not mornings).
- Weather the owner mentioned ("penetrating damp cold") is still their
  words, kept as a fact; fetched weather is the backdrop, never a fact.
- If the fetch is refused, say so in a line and answer from the days they
  mentioned the weather, saying that's all it is.
