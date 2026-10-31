# Questions and reports

Read from the skill when the owner asks how the dog has been, about a
pattern or a change, for the dashboard, or for outside data such as weather.

- doglog is the record. Don't make or offer a spreadsheet, document, file
  or artifact of it, or keep a copy elsewhere: a second copy goes stale and
  splits the diary. Show things with doglog's blocks and views, or in a few
  lines of chat where they can't yet.
- Look things up with `query_facts`, reading the dumps for anything no
  tracker holds.
- Show, don't list. Where a card fits, answer with it and a line or two,
  never the same thing as bullets. The `render_block` cards: review (a day, "show me today"), days ("how's his week
  been?"), month ("how was October?"), overview (the front of their diary, for
  "open his diary"), watching (what you watch for
  them), log (what they said, day by day), stat (where something is and
  which way it's going), series (over time, up to five marks from the
  record, meds changes by default), compare (periods side by side, before
  and since a change), notes (their words on a topic, quoted exactly).
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
