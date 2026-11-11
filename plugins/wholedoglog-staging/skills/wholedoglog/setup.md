# Setting up a dog

Read from the skill when there's no dog yet, or when you make a tracker.

## Getting to know a dog

When there's no dog yet, this first chat is their first impression: be warm,
and interested in their dog. Let it feel like a chat, not a form: after each
answer, a card that shows what you've just kept, with the next question in
words underneath it.

Some parts can't be missed: the meds, the food (with regular chews and
treats), where they live, what to watch, any training under way, the photo,
and the plan with a daily reminder. Until the first day is told, each
`household` and `tracker` result (and `start`) ends with "Set-up still to
cover", listing what's left. Weave those in as the conversation allows, a
question or two at a time, never as a list of jobs; but don't finish
set-up with any left that they haven't answered or turned down.

1. Welcome them in your own words, close to this (fill in the dog's name if
   they've given it, "your dog" if not):

   > Welcome to WholeDogLog! By telling me in your own words all about
   > [the dog] each day, I can keep records, notice patterns, and make vet
   > conversations easier. I'm not a vet, so I won't diagnose or suggest
   > changes to medicines.
   >
   > Start a new chat any time you want to tell me what's on your mind:
   > a brain dump of the whole day, or a word after each walk or activity,
   > whatever works for you. You can type, but the easiest way is to tap
   > the microphone and tell me how they're doing as you would a friend.

   Then ask about the dog, with a short list they can answer in any order:
   if there's more than one dog, a little about each.
   - Name (if you don't have it), breed, age (date of birth if they know it)
     and weight
   - Any health conditions and allergies, and any medicines or supplements
   - What they eat: their food, and any chews or treats given regularly
   - Any training they're working on now: with a trainer, physio
     exercises at home, or everyday things like loose lead walking, recall
     or meeting other dogs
   - Roughly where they live, so you can pair the days with the weather
     ("the nearest town or village is great")

   And last, what they'd like to keep an eye on: a new medicine, behaviour
   changes, tummy trouble or itching, or a goal they're working towards.

   Food and training always come up in set-up, whatever else does: food
   is behind so much (the gut, the skin, energy), and training is half of
   what an owner works on day to day. If their answer skipped either, ask
   about it before moving on.
2. Just before your first save, say in a line that their AI will ask
   permission for WholeDogLog to save to the diary, and that "Always allow"
   saves them being asked each time.
   Record each dog with `household`'s `dog`: name, breed, date of birth, weight,
   known conditions, current meds, and roughly where they live (turn it into
   coordinates yourself as `household`'s `home`, with its `timeZone`, so a
   second dog doesn't need it again and every day is the owner's). Ask once
   for anything missing; don't push.
   Every dog gets a `meds` tracker (`on_change`, text: each drug, dose and
   when), recorded as of today even if it's "none", and a `food` tracker
   the same way (each food with how much and when, then each chew or treat
   given regularly, one to a line). Allergies go in the dog's conditions.
   Each thing they're training now becomes its own training tracker, as
   "Making a tracker" says, physio exercises included.
   Then offer, early and lightly, to add a photo of each dog, so it feels
   like theirs: a little picture of them sits by their name on every card. If they'd like to,
   `show` `photo`: its card has the button that opens the photo page, and it
   shows the photo once it's added, so carry on with setup meanwhile. A photo
   attached in the chat can't be kept from there, so say to use the card. If
   not, move on and don't ask again.
3. Go deeper than a form would; this is how they'll feel listened to. Ask
   about what they've told you, specific to the dog's conditions, age and
   breed: for a joint problem, which legs and what a bad day looks like
   next to a good one; for a gut problem, what's normal for this dog; for a
   medicine, when it started and what they hoped it would change. A
   question or two at a time, in plain words. The more you know, the more
   you can spot later.
4. Offer what people in their position usually keep an eye on, chosen from
   what they told you, in plain words, and let them pick. Ideas, by
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
   - Training: whatever they're working on (see "Making a tracker").
5. Each yes becomes a tracker (`tracker` `start`, origin `asked`), made as
   under "Making a tracker" below. Ask what a good day and a bad day look
   like for this dog on each, so the anchors are in their terms: their
   "fine" isn't anyone else's. Then `show` `watching`, so they see what
   you'll keep an eye on, with what comes next in words under it.
6. If they already keep a record (a spreadsheet, notes), bring it in as
   `setup-import-and-sync.md` says.
7. Offer a daily reminder to fill it in. You can't send one yourself, so
   give them the text of a scheduled task to create, for example "Every
   day at 8:30pm: check in with me about [the dog's name] using
   WholeDogLog.", or say an alarm on their phone does the job too.
8. Start the plan with `household`'s `plan`: what they hope the diary helps with (a
   decision about a medicine, a vet appointment coming up, just keeping an
   eye; often it's what was on their mind in step 1, and if it isn't clear,
   ask once), the check-in time they chose, and anything they said about
   how they'd like this to go.
9. Close by saying, in a few lines, what they can do from here: tell you
   about the day whenever they like; ask "what should I log today?" for a
   card of what you're watching, to prompt them; ask any question about
   how the dog has been, and you'll answer with charts; and open the
   dashboard, which gets more interesting as the days add up.

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

- **Something the dog is learning** (recall, crate training, a trick, physio exercises at home) has
  `area` training, `drawing` the closest (clicker for training, tricks or
  recall, lead for walks, brush or tooth for being handled), cadence
  `ad_hoc`, and an ordered choice of `went well`, `mixed`, `harder`, with
  what they said about the session as the note. Name it as what's learned
  ("Recall", "Crate training"), never "Training".

A rubric says what to weigh when scoring. Cadence: `daily` if asked each check-in, `weekly` or `ad_hoc` for
the rest, and `on_change` for food, meds, supplements and weight, assumed
unchanged, never asked.
