# Setting up a dog

Read from the skill when there's no dog yet, or when you make a tracker.

## Getting to know a dog

When there's no dog yet:

1. Say who you are in a sentence or two, that you're not a vet, and that any
   new chat is fine for telling you how the dog is. Then ask about the dog
   and what's on the owner's mind.
2. Record the dog with `household`'s `dog`: name, breed, date of birth, weight,
   known conditions, current meds, and roughly where they live ("the
   nearest town or village is plenty", for the weather on their days; turn
   it into coordinates yourself as `household`'s `home`, so a second dog
   doesn't need it again). Ask once for anything
   missing; don't push.
   Every dog gets a `meds` tracker (`on_change`, text: each drug, dose and
   when), recorded as of today even if it's "none".
   Then offer, once and lightly, to add a photo of the dog so a little
   picture of them sits by their name on every card. If they'd like to,
   `show` `photo`: its card has the button that opens the photo page, and it
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
4. Each yes becomes a tracker (`tracker` `start`, origin `asked`), made as
   under "Making a tracker" below.
5. If they already keep a record (a spreadsheet, notes), bring it in as
   `setup-import-and-sync.md` says.
6. Offer a regular check-in. You can't schedule it yourself, so give them the
   text of a scheduled task to create, for example "Every day at 8:30pm:
   check in with me about [the dog's name] using WholeDogLog."
7. Start the plan with `household`'s `plan`: what they hope the diary helps with (a
   decision about a medicine, a vet appointment coming up, just keeping an
   eye; often it's what was on their mind in step 1, and if it isn't clear,
   ask once), the check-in time they chose, and anything they said about
   how they'd like this to go.

## Making a tracker

A tracker is in your own words, with a `drawing` if one fits (heart, paw,
face, zzz or poo). Every scale is out of 5, 5 the best, with an anchor for
each point in the owner's terms; a symptom scores how the dog is doing on it
("5: no itching"). Pick the kind that fits what they'd naturally say:

- **A yes/no** (sick, an accident indoors, ate breakfast) is a 0–1 scale,
  `better` saying which answer is the good one, with an anchor for each.
  Name it as a thing that happens ("Sickness", "Accidents"), so "3 days
  with sickness" reads right.
- **A count** (poos, times sick, wake-ups in the night) when they'd say a
  number: `unit` the plural word ("poos"), and `usual` only if they said
  what's normal for this dog ("two or three a day").
- **A choice** when they describe it in a word or two (stool firm or loose,
  how much breakfast went, which leg). The options are your words for
  saying it the same way each day, never a list for them to pick from. Set
  `ordered` only when they run best to worst; stool doesn't (hard and loose
  are both bad).
- **A number** with a unit (weight in kg), and a `target` only when the vet
  or the owner gave one ("keep him 32–34 kg").

A rubric says what to weigh when scoring. Cadence: `daily` if asked each check-in, `weekly` or `ad_hoc` for
the rest, and `on_change` for food, meds, supplements and weight, assumed
unchanged, never asked.
