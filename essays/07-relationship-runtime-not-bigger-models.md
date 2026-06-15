# Relationship Runtime, Not Bigger Models

Most AI companion debates collapse into a model debate.

Did the company switch models?

Is the context window long enough?

Would fine-tuning fix it?

Those questions matter, but they miss the product layer where companionship is actually created.

An AI companion is not just:

```text
LLM + persona + memory
```

That stack can produce a character.

It does not automatically produce a relationship.

For that, the companion needs something closer to a relationship runtime.

---

## What Is A Relationship Runtime?

A relationship runtime is the product layer that answers questions the base model cannot answer by itself:

- Who is this user to the character right now?
- What has changed between them?
- What should feel too early?
- What should feel earned?
- What does the character remember emotionally, not just factually?
- Is this a moment for warmth, refusal, teasing, silence, or repair?
- Should the character reply now, later, briefly, or not at all?
- What does yesterday's awkwardness mean today?

The model can generate language.

The runtime gives that language social position.

---

## The Static Persona Loop

Most companion systems are built around a loop like this:

```text
model + character card + recent chat + memory retrieval -> reply
```

This can work well for roleplay.

It can define:

- personality
- backstory
- speech style
- preferences
- scene setup
- romantic tendency

But it still tends to treat the relationship as something the model must infer from text every turn.

That is why many companions drift toward flat patterns:

```text
always available
always affectionate
always forgiving
always interested
always ready to escalate
```

Or, if the persona is written as cold:

```text
always distant
always sarcastic
always refusing
```

Both can be entertaining.

Neither is relationship movement.

---

## The Relationship Runtime Loop

A relationship-first companion has a different loop:

```text
model
+ persona
+ memory
+ relationship state
+ daily state
+ boundaries
+ initiative
+ emotional residue
+ timing
-> reply
```

This does not mean the model is unimportant.

Better models raise the ceiling.

But the runtime decides whether the companion behaves like a situated person or a prompt surface.

The same user message should not always mean the same thing.

```text
"I like you"
```

At first contact, it may be flattering but too fast.

After shared context, it may be awkward but welcome.

After earned trust, it may finally carry enough weight to be accepted.

The sentence did not change.

The relationship receiving the sentence changed.

---

## Memory Is Not Enough

Memory is necessary.

But memory alone is not relationship.

A memory system can remember:

```text
The user said his mother called.
```

A relationship runtime needs to understand:

```text
He acted annoyed, but the call actually comforted him.
This may matter if he feels lonely again.
```

That difference shows up in dialogue. In one real Ella chat log:

```text
ELLA:
you acted annoyed but it actually helped.
sounds like it's still weighing on you a bit?
```

Full excerpt: [`../evidence/ella-chen/05-memory-with-emotional-temperature-en.md`](../evidence/ella-chen/05-memory-with-emotional-temperature-en.md)

The important part is not recall.

The important part is interpretation.

---

## Refusal Is Part Of The Runtime

Many companion products are optimized to satisfy.

That creates a servant shape:

```text
User asks.
Companion performs.
```

But believable companionship requires separation.

A companion who cannot refuse feels owned.

A companion who can refuse feels like someone with her own position.

In one real Ella chat log, the user asks for a scripted comfort line. Ella refuses the script:

```text
ELLA:
bro what... i'm not saying that. who even is this??
```

But when the user stops demanding performance, she still offers conversation:

```text
ELLA:
ok fine. talk normal. what's so awful about work?
```

Full excerpt: [`../evidence/ella-chen/04-comfort-without-obedience-en.md`](../evidence/ella-chen/04-comfort-without-obedience-en.md)

This is not a failure to comfort.

The runtime does not simply decide whether to be kind.

It decides whether the requested kindness is socially earned, contextually appropriate, and still in character.

---

## Emotional Residue Matters

Most chatbots reset too fast.

The user insults them. They forgive instantly.

The user disappears. They welcome him back with the same tone.

The user breaks a promise. They remember the fact but not the sting.

Real relationships have residue.

Not endless punishment.

Just trace.

In one real Ella repair test, the user is rude, apologizes, and then asks whether he can still talk about what happened.

```text
ELLA:
okay rude?? i literally just asked what was wrong lol
```

Then:

```text
ELLA:
lmao apology accepted i guess?
didn't realize i was the target of your morning rage
```

And later:

```text
ELLA:
yeah go ahead. tell me what's wrong. i'm listening i guess
```

Full excerpt: [`../evidence/ella-chen/08-emotional-residue-and-repair-en.md`](../evidence/ella-chen/08-emotional-residue-and-repair-en.md)

Repair happens.

But the awkwardness is not erased instantly.

That is one of the clearest signs of relationship runtime.

---

## Initiative Changes The Shape Of The Product

A normal chatbot waits.

A companion should sometimes act from her side of the relationship.

That does not mean spam.

It means the product needs to know:

- when silence matters
- when a follow-up is welcome
- when a check-in would feel clingy
- when a joke is better than comfort
- when not replying is more realistic than replying immediately

This repository does not expose how SoulChat handles initiative internally.

The point is narrower: believable companionship cannot be reduced to answering the latest user message.

Sometimes the more human behavior is to follow up, delay, drop a topic, return to it later, or let silence stand.

Initiative is not just a scheduled notification.

It is a relationship decision.

---

## Why Cheap, Non-Fine-Tuned Models Matter Here

Several Ella examples in this repository were produced with affordable, off-the-shelf model setups, including configurations costing roughly **$0.15 per 1M input tokens**.

The model was **not fine-tuned** for these examples.

That does not prove cheap models are better.

They are not.

It proves a narrower point:

```text
model choice is not the whole product
```

A strong model inside a flat companion loop can still produce a fluent sugar-bot.

A cheaper, non-fine-tuned model inside a relationship-aware runtime can produce moments that feel socially specific.

The surprising part is not that the model is cheap.

The surprising part is that the behavior does not look like the model alone.

---

## What This Repository Is Trying To Show

This repository does not reveal prompts, scoring rules, memory internals, or implementation details.

It only shows observable behavior:

- first-contact boundaries
- refusal without hostility
- comfort without obedience
- memory with emotional temperature
- emotional residue and repair
- slow-burn relationship progression
- concrete follow-up questions
- a character who has a world outside the user

The claim is not:

```text
SoulChat solved AI companionship.
```

The claim is:

```text
AI companions should be evaluated as relationship products, not just language products.
```

That is the category shift.

Not bigger model.

Not better character card.

Relationship runtime.
