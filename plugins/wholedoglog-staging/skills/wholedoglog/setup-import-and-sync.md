# Bringing in an old record, and keeping their sheet

Read from the skill when they have an old record to bring in (a spreadsheet,
notes), or a Google Sheet to keep up to date.

## Bringing it in

Read it on your side, say back what each column becomes in their terms, and
fix anything that reads the wrong way round (a "pain" score where 5 means
comfortable). Dates go in as YYYY-MM-DD; ask if one is ambiguous. Make the
trackers it fills in first.

A Google Sheet brought in is also kept up to date from then on (below): say
so in a line, unless they say they'd rather not.

It goes in as one import, with one card:

1. Say it takes a few minutes and the card shows how it's going.
2. `show` `import`: what they call it ("Bramble's sheet") and
   its first and last day.
3. `record` with the same `import`, oldest first, about three weeks a
   call, a row per day: its notes as given, each tracker's value by key
   (`"values": {"sleep": 4, "stool": "firm"}`), anything notable as
   `events`. A `key` per call; `last: true` on the last. A blank day stays
   blank.
4. Say nothing between calls and show no other cards. Fix refusals in the
   next call; only ask about what you can't work out.

Once it's done the card shows what came in, with days that open the diary.
Then: a line on what came in; a check-in time if the plan has none (the text
of a scheduled task, as in `setup.md`); and if today is empty, offer to do
today now, or else show the last recorded day's `review`. Never leave them
on a summary with nowhere to go.

## Keeping their sheet up to date

They should never tell you a day twice: you record it here, then fill in
their sheet too.

1. Look at it through their own Sheets connector. If this chat can't reach
   it, say which connector they'd need, in a line, and carry on.
2. Work out how to fill it in from the conventions written in the sheet,
   its recent rows, and what they tell you ("only the log tab"). If
   something isn't clear, ask.
3. `household` with `sheet` (its link and name), and its `plan` saying how to fill it in
   under the sheet's name: the tab, a row per day or not, each column and
   how you score it, what to leave alone. Enough for a later chat to do it
   without reading the sheet's notes.

Each check-in then updates it, following the plan. When they change how they
want it done, or the sheet changes, update the plan. It's their sheet: do it
their way. `household`'s `sheet` with `unlink` stops it; take its section out of the
plan too.
