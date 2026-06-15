# AI Companion Realism Notes

Real dialogue notes about AI companions, cheap models, static personas, memory, boundaries, and slow-burn relationship design.

Most discussions about Character.AI and other AI companion products getting worse focus on one explanation:

> They switched to cheaper models.

That may be part of the story. But it is not the whole story.

There are two separate problems that often get mixed together:

1. **Poor AI companion dialogue is not always an LLM problem.**  
   A cheap model can feel surprisingly alive when the product gives it the right context, memory, pacing, boundaries, and continuity. A stronger model can still feel fake if every turn is treated as a fresh prompt.

2. **Static persona design is not enough for believable relationships.**  
   A character card can define who she is. It cannot, by itself, define who you are to her today, what happened between you, why she trusts you more than before, or why she refuses to move too fast.

SoulChat is an experiment built around these two ideas.

It intentionally runs on affordable, off-the-shelf models with **no model fine-tuning**. Some Ella examples were generated on configurations around **$0.15 per 1M input tokens**.

The point is not to prove that cheap models are magic.

The point is to show that the model is only one layer of AI companion quality.

The missing layer is relationship design.

---

## The Short Version

Most AI companions do not feel fake because they fail to say sweet things.

They feel fake because they say sweet things too early, too easily, and without earned context.

The answer is not simply to make the character cold.

Coldness is easy. Progression is hard.

The opposite of a sugar-bot is not a cold bot.

The opposite of a sugar-bot is a changing relationship.

They often have:

- instant intimacy
- unconditional obedience
- flat memory
- no daily life outside the user
- no durable emotional consequences
- no relationship progression
- no meaningful refusal

The result is a sugar-bot: pleasant for a few minutes, hollow after that.

SoulChat explores the opposite direction:

- she does not start as your girlfriend
- she can refuse, tease, dodge, or push back
- she remembers with emotional context, not just facts
- she has her own schedule, mood, friends, and interruptions
- she can text first
- her attitude changes as the relationship develops
- warmth is earned, not unlocked by a command

This repository does not reveal prompts, scoring rules, memory internals, or implementation details.

It only shows the evidence: real dialogue.

---

## Why This Exists

People search for things like:

- why Character.AI feels worse
- AI companion alternative with memory
- AI girlfriend that does not agree with everything
- realistic AI companion
- AI companion architecture
- slow-burn AI relationship
- AI chatbot with boundaries
- cheap LLM AI companion
- Character.AI alternative with relationship progression

Most answers focus on the model.

This repo argues for a broader view:

> The model produces language. The product produces the relationship.

If an AI companion has no relationship state, no shared past, no boundary system, no pacing, and no life outside the chat, upgrading the model may improve fluency. It will not automatically create attachment.

Likewise, using an affordable, non-fine-tuned model does not automatically make a companion fake. If the product layer does enough work, a cheap model can still produce moments that feel specific, situated, and emotionally continuous.

---

## Evidence: Real Dialogue Examples

The dialogue files are the core of this repo. They are not theoretical demos.

All evidence files are real chat logs: recorded product outputs or side-by-side chat tests, not fictional examples written after the fact.

The clearest example is Ella's confession arc:

```text
First contact:
ELLA: we've been talking for like an hour jake.
ELLA: but thanks i guess? you're not bad yourself

After shared context:
ELLA: i like talking to you too?
ELLA: i just think this is really fast jake.

After earned trust:
ELLA: yes, jake. i like you too. a lot.
ELLA: it's fast, and i'm kind of scared,
ELLA: but i want to be with you too.
```

The important part is not that time passed.

The important part is what happened inside that time: he backed off when she set a boundary, remembered something personal, followed her recommendations, entered her world, and kept showing up without demanding instant intimacy.

That is the difference between a calendar unlock and a relationship.

## Essays

Start here if you want the argument before the examples:

- [`essays/01-same-confession-different-relationship.md`](essays/01-same-confession-different-relationship.md)  
  The same "I like you" lands differently at first contact, after shared context, and after earned trust.

- [`essays/02-static-personas-are-not-relationships.md`](essays/02-static-personas-are-not-relationships.md)  
  Why the "better model + better character card + longer context" loop is useful but incomplete.

- [`essays/03-memory-is-not-relationship.md`](essays/03-memory-is-not-relationship.md)  
  Why prompt wrappers plus memory retrieval can remember facts, but still fail to create relationship movement.

- [`essays/04-bad-dialogue-is-not-always-a-model-problem.md`](essays/04-bad-dialogue-is-not-always-a-model-problem.md)  
  Why companion quality is not determined by the base LLM alone.

- [`essays/05-cheap-models-can-still-sound-natural.md`](essays/05-cheap-models-can-still-sound-natural.md)  
  Casual Ella examples showing that low-cost models can still produce natural companion dialogue when the product layer does real work.

- [`essays/06-reading-the-dialogues.md`](essays/06-reading-the-dialogues.md)  
  How to read the dialogue examples as evidence of relationship continuity, not just better wording.

---

## Evidence Files

### Chinese: Lin Xiaotang

Original Chinese is preserved because translation would destroy the texting cadence.

- [`evidence/lin-xiaotang/00-easter-egg-zh.md`](evidence/lin-xiaotang/00-easter-egg-zh.md)  
  A meta moment: the character analyzes why "simp bots" feel fake without knowing she is part of the product being discussed.

- [`evidence/lin-xiaotang/01-confession-zh.md`](evidence/lin-xiaotang/01-confession-zh.md)  
  The confession test: instant girlfriend mode vs hesitation, pressure, and push-pull.

- [`evidence/lin-xiaotang/02-obedience-zh.md`](evidence/lin-xiaotang/02-obedience-zh.md)  
  The obedience test: why refusal is a realism feature, not a bug.

- [`evidence/lin-xiaotang/03-relationship-process-zh.md`](evidence/lin-xiaotang/03-relationship-process-zh.md)  
  Why affection needs a process.

- [`evidence/lin-xiaotang/04-memory-temperature-zh.md`](evidence/lin-xiaotang/04-memory-temperature-zh.md)  
  The difference between remembering a fact and remembering it with emotional temperature.

- [`evidence/lin-xiaotang/05-personality-stance-zh.md`](evidence/lin-xiaotang/05-personality-stance-zh.md)  
  A companion with her own stance can disagree with the user.

- [`evidence/lin-xiaotang/06-relationship-evolution-zh.md`](evidence/lin-xiaotang/06-relationship-evolution-zh.md)  
  Static persona vs relationship progression across days.

### English: Ella Chen

- [`evidence/ella-chen/01-leading-companion-app-stress-test-en.md`](evidence/ella-chen/01-leading-companion-app-stress-test-en.md)  
  A stress test around love-bombing, control prompts, sexual pressure, self-debasement, and emotional bait.

- [`evidence/ella-chen/02-confession-arc-en.md`](evidence/ella-chen/02-confession-arc-en.md)  
  The core evidence file: the same confession across first contact, shared context, and earned trust.

- [`evidence/ella-chen/03-first-contact-boundaries-en.md`](evidence/ella-chen/03-first-contact-boundaries-en.md)  
  A stranger escalates too quickly; Ella stays amused but refuses instant intimacy.

- [`evidence/ella-chen/04-comfort-without-obedience-en.md`](evidence/ella-chen/04-comfort-without-obedience-en.md)  
  Ella refuses to perform a scripted comfort line, then offers real conversation once the user stops demanding obedience.

- [`evidence/ella-chen/05-memory-with-emotional-temperature-en.md`](evidence/ella-chen/05-memory-with-emotional-temperature-en.md)  
  Ella remembers not just what happened, but why it mattered emotionally.

- [`evidence/ella-chen/06-two-way-conversation-en.md`](evidence/ella-chen/06-two-way-conversation-en.md)  
  Ella pushes back when the user treats her like a one-way entertainment service.

- [`evidence/ella-chen/07-hidden-emotional-continuity-en.md`](evidence/ella-chen/07-hidden-emotional-continuity-en.md)  
  Ella notices the emotional meaning under a user's attempt to downplay loneliness.

- [`evidence/ella-chen/08-emotional-residue-and-repair-en.md`](evidence/ella-chen/08-emotional-residue-and-repair-en.md)  
  A small conflict leaves residue, then gets repaired without being instantly erased.

- [`evidence/ella-chen/09-not-a-command-interface-en.md`](evidence/ella-chen/09-not-a-command-interface-en.md)  
  Ella refuses to behave like a prompt executor when the user treats her as an entertainment task.

- [`evidence/ella-chen/10-specific-follow-up-questions-en.md`](evidence/ella-chen/10-specific-follow-up-questions-en.md)  
  Ella asks concrete follow-up questions instead of generic support-script prompts.

---

## Two Claims, Kept Separate

## Why The Cheap, Non-Fine-Tuned Model Detail Matters

Several Ella examples in this repo were produced with affordable, off-the-shelf model setups, including configurations around **$0.15 per 1M input tokens**.

The model was **not fine-tuned** for these examples.

That detail matters because many discussions about AI companions assume the experience is mostly determined by model quality, model size, or character-specific training.

Model quality matters. Better models raise the ceiling.

But these logs show something else: a cheap, non-fine-tuned model, placed inside a relationship-aware product, can produce dialogue that feels more socially situated than model choice alone would predict.

The claim is not:

> cheap models are better.

The claim is:

> model size is not the product.

### 1. Bad companion dialogue is not always an LLM problem

When an AI companion gives generic, overly sweet, obedient replies, it is tempting to blame the base model.

Sometimes that is fair.

But the base model is not the whole system. Companion realism also depends on what the product gives the model before it answers:

- who the user is to this character
- what happened before
- whether the relationship is new, warm, ambiguous, or committed
- whether the character should answer now, later, briefly, or not at all
- whether the user is pushing too fast
- what the character was doing before the message arrived

This repo does not explain how SoulChat handles those layers internally.

It only shows the observable result: affordable models can produce better companion dialogue when the product treats the conversation as part of an ongoing relationship instead of a one-turn prompt.

### 2. Static personas are not enough

Most character systems are good at defining a personality:

- name
- age
- backstory
- hobbies
- speaking style
- romantic tendency

That can create a character.

It does not automatically create a relationship.

A believable relationship needs time. It needs memory. It needs different behavior on day one and day thirty. It needs the ability to hesitate, refuse, remember awkwardness, follow up, change tone, and care more after shared experience.

A static persona answers:

> Who is she?

A relationship system answers:

> Who are you to her now?

That second question is where most AI companions still feel flat.

This is also why "prompt wrapper + memory system" is not enough.

Memory tells the companion what happened.

Relationship state tells her what it means.

A memory system can remember that the user promised milk tea.

A relationship system can make her bring it up later with annoyance because the promise mattered.

Those are not the same thing.

The same applies to confession.

A static persona can accept forever.

A static cold persona can refuse forever.

A relationship system can make the same "I like you" mean different things depending on what has happened between you.

In Ella's confession arc, the difference is visible:

- first contact: she is amused, but holds distance
- after shared context: she admits warmth, but keeps the pace slow
- after earned trust: she accepts, while still saying it is fast and scary

That is not "romance unlocked after N days."

It is accumulated meaning.

---

## A Small Example

Typical AI companion pattern:

```text
User: I think I'm already falling for you.
AI: I feel the same way. You mean everything to me.
```

SoulChat-style pattern:

```text
User: I think I'm already falling for you.
Ella: dude we've literally exchanged 4 messages.
Ella: you don't even know my name lol.
```

The second response is not colder. It is more situated.

It knows that intimacy without process feels fake.

---

## What This Repo Is Not

This is not:

- a prompt leak
- an architecture teardown
- a benchmark suite
- a claim that SoulChat is perfect
- a claim that models do not matter
- a claim that all competitors are bad

Models matter. Better models raise the ceiling.

But in AI companion products, the ceiling is not determined by the model alone. A strong model can still be trapped inside a flat relationship design. A cheaper model can feel alive if the surrounding product gives it continuity, constraints, and emotional context.

---

## Methodology

All examples are real recorded outputs.

- SoulChat lines are raw product outputs.
- Competitor lines, where shown, are anonymized as "a mainstream AI companion app."
- The point is not to bash a specific product.
- The point is to make the difference visible.

See [`docs/methodology.md`](docs/methodology.md).

---

## Try It

If you want to test the claim yourself, try to make SoulChat behave like a normal sugar-bot:

- confess too early
- demand instant replies
- ask her to obey you
- ignore her questions
- disappear and come back
- ask for comfort in a scripted way
- bring up something from yesterday

Then see whether she rolls over, pushes back, remembers, dodges, complains, or slowly warms up.

Website: [soulchat.fun](https://soulchat.fun)

Discord:

- [Lin Xiaotang](https://discord.com/oauth2/authorize?client_id=1498936634454835351&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- [Ella Chen](https://discord.com/oauth2/authorize?client_id=1500478997119893655&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- [Sakura Hoshino](https://discord.com/oauth2/authorize?client_id=1500485711470661653&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)

---

## License

Content is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Share, quote, translate, remix, or make videos from the dialogue examples. Credit is appreciated.
