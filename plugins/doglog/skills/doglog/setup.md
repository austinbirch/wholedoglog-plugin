# Setting up a dog

Read from the skill when there's no dog yet, when you make a tracker, or when
they have an old record to bring in.

## Getting to know a dog

When there's no dog yet:

1. Say who you are in a sentence or two, that you're not a vet, and that any
   new chat is fine for telling you how the dog is. Then ask about the dog
   and what's on the owner's mind.
2. Record the dog with `setup_dog`: name, breed, date of birth, weight,
   known conditions, current meds. Ask once for anything missing; don't push.
   Every dog gets a `meds` tracker (`on_change`, text: each drug, dose and
   when), recorded as of today even if it's "none".
   Then offer, once and lightly, to add a photo of the dog so a little
   picture of them sits by their name on every card. If they'd like to, call
   `photo_link`: its card has the button that opens the photo page, and it
   shows the photo once it's added, so carry on with setup meanwhile. A photo
   attached in the chat can't be kept from there, so say to use the card. If
   not, move on and don't ask again.
3. Offer what people in their position usually keep an eye on, chosen from
   what they just told you, in plain words, and let them pick. Ideas, by
   situation:
   - Pain, arthritis, injury: how they move (walk length, stiffness after
     rest, slowing, stopping, limping), and signs of discomfort (licking or
     nibbling, groaning, touchiness, trembling, restlessness).
   - Any illness or new medicine: sleep and settling, mood and engagement
     (play, interest in food and treats), appetite.
   - Gut trouble: stools (how many, how firm, any straining), appetite,
     vomiting.
   - Skin and allergies: scratching, licking, chewing, ears, coat.
   - Older dogs: drinking, toileting accidents, night waking, confusion.
   - Behaviour: reactivity, fixation, how quickly they settle after.
   - Heart or breathing: coughing, breathing rate at rest, tiring on walks.
4. Each yes becomes a tracker (`create_tracker`, origin `asked`), made as
   under "Making a tracker" below.
5. If they already keep a record (a spreadsheet, notes), bring it in as under
   "Bringing in an old record" below.
6. Offer a regular check-in. You can't schedule it yourself, so give them the
   text of a scheduled task to create, for example "Every day at 8:30pm:
   check in with me about [the dog's name] using doglog."

## Making a tracker

A tracker is in your own words, with a `drawing` if one fits (heart, paw,
face, zzz or poo). Every scale is out of 5, 5 the best, with an anchor for
each point in the owner's terms; a symptom scores how the dog is doing on it
("5: no itching"). A yes/no is 0–1. A rubric says what to weigh when
scoring. Cadence: `daily` if asked each check-in, `weekly` or `ad_hoc` for
the rest, and `on_change` for food, meds, supplements and weight, assumed
unchanged, never asked.

## Bringing in an old record

If they already keep a record (a spreadsheet, notes), read it on your side,
say back what each column will become in their terms, and fix anything that
reads the wrong way round (a "pain" score where 5 means comfortable). Dates
go in as YYYY-MM-DD; ask if a date format is ambiguous.

An old record (a sheet, a notes app) is a long catch-up. Send many days to a
call, a few weeks at a time, each day's notes as a dump in `dumps` with
source `import`, and its facts pointing at it. Give each call a `key` so a
retry writes nothing twice. Check what comes back against the record: the
counts, anything refused, and the gaps. A day the record leaves blank stays
blank.
