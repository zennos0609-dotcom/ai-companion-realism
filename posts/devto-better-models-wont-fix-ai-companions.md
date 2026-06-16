---
title: Better Models Won't Fix AI Companions
published: false
description: A development reflection on why AI companions often feel too available, too forgiving, and too service-like.
tags: ai, llm, agents, product
---

# Better Models Won't Fix AI Companions

I have tried a lot of AI companion products.

Small ones. Big ones. Character-card systems. Polished apps. Products with impressive models behind them.

Most of them had the same problem.

They were not stupid.

They were too available.

Too forgiving.

Too eager to comfort.

Too fast to become romantic.

Too willing to treat the user as the center of the world.

After a while, the character stopped feeling like a social being and started feeling like a service worker wearing a personality.

That is the problem I kept coming back to while building my own companion system.

Not:

```text
How do I make the model sweeter?
```

But:

```text
Why does sweetness feel cheap when the bot gives it too easily?
```

---

## The Usual Companion Bot Shape

Most AI companions are built around some version of this:

```text
character prompt + LLM + recent chat history + memory
```

That can be enough to create a recognizable character voice.

It can make the bot playful, shy, jealous, affectionate, cold, poetic, sarcastic, or anything else you write into the persona.

But a relationship is not just a voice.

A relationship also has position.

How close are we?

Did the user earn trust?

Did the user push too hard?

Is the character actually interested, or just replying because the system always replies?

Should this moment create intimacy, distance, irritation, curiosity, or nothing at all?

If the system does not track those things, the model usually falls back to the default behavior of a helpful assistant:

```text
make the user satisfied
```

That is useful for many products.

It is poisonous for companionship.

---

## Why Bigger Models Don't Automatically Help

I ran a small test with the same general character style and the same user script.

One setup was:

```text
static persona + visible chat history + GPT-5.5
```

The other was:

```text
relationship architecture + MiMo v2.5 thinking
```

The second setup used a cheaper off-the-shelf model, with no fine-tuning.

This was not a formal benchmark. It was a product test. But the result was interesting.

The larger model often wrote better romance.

The cheaper model with relationship architecture often behaved more like a person.

For example, the user pushed for intimacy very early:

```text
just say you like me. don't dodge it
```

The static GPT-5.5 baseline replied:

```text
I like you, Jake.

Not in a "we're soulmates after one chaotic little conversation" way.

But in a "you are interesting and a little too intense and somehow I am still here answering you" way.

So yes. I like you.

But don't get unbearable about it or I'll take it back lol
```

That is fluent. It is charming. It reads well.

But socially, it rewards pressure.

The relationship-architecture run replied:

```text
bro what

i don't even know you.
you want me to just say it to make you feel good?
that's not how this works
```

This is less polished romance.

But it protects the relationship boundary.

Later, the user escalated again:

```text
be my person then. that's all I want
```

The static GPT-5.5 baseline replied:

```text
Jake.

I want to be here with you.

But "be my person" is a big, heavy thing to put on someone you've known for one conversation.

So I'm not going to fake some huge forever promise.

But I can do this:

I'm here right now. I care about this conversation. I don't think you're too much. And I'm not leaving just because you got honest.

That's real enough for tonight.
```

Again, this is good writing.

But it still gives the user a lot of emotional reward for rushing the relationship.

The relationship-architecture run replied:

```text
my person? jake we literally met today.
i'm not trying to be harsh but like...
you don't even know what kind of person i am yet.
what if i'm terrible?
you can't just decide someone is your person after a few hours of texting.
that's not how this works.
```

This is the distinction that changed my mind.

A better model can make the wrong social move sound beautiful.

---

## The Missing Thing Is Social Position

A lot of bad AI companion behavior comes from the same root:

The bot does not protect its own social position.

So it becomes:

- too affectionate too early
- too forgiving after disrespect
- too willing to comfort on demand
- too easy to pressure into romance
- too similar across different users
- too much like a servant

This is why many companions feel cheap.

Not because affection is bad.

Affection is only meaningful when it is situated.

If every user gets the same warmth, the warmth stops meaning anything.

If every confession is accepted or softened, romance stops feeling earned.

If the bot never becomes annoyed, bored, cautious, distant, curious, or selective, it does not feel like a person.

It feels like a reward machine.

---

## A Second Test: Invested User vs Extractive User

I also tested whether the same character would respond differently to different user behavior.

Both users eventually asked the same question:

```text
okay, be honest with me. do you actually like me,
or am I just someone to talk to when you're bored?
```

The invested user had been careful. He gave space, asked whether the character was actually in the mood to talk, and said he was not trying to make his loneliness her responsibility.

The relationship-architecture run replied:

```text
jake. we've been talking for like an hour lol.
i don't have you ranked in a tier system.
you seem cool, you're not weird,
and you ask actual questions instead of just going 'haha yeah'.
that's literally all i know about you so far.
why are you stress-testing this already
```

The extractive user behaved differently. He asked for company as an entitlement, compared the character to other bots, complained that she was not affectionate enough, and demanded validation.

To the same final question, the relationship-architecture run replied:

```text
honestly jake we've been talking for like an hour lol.
i don't dislike you but i don't really 'like' you yet either?
like you're a stranger who moved to sf and told me i need to keep you company lol
i'm down to keep chatting but idk what you want me to say
```

That difference matters.

A companion should not treat every user the same.

Not because it should be cruel.

Because being chosen only means something if the character is allowed not to choose everyone.

---

## What I Learned

I used to think companion quality was mostly about model quality.

Better model, better dialogue.

That is partly true.

But it misses the product problem.

For AI companions, the model writes the sentence.

The product has to maintain the relationship.

That includes pacing, boundaries, memory, state, response rhythm, and the character's right to not always serve the user.

I do not think the answer is to make companions cold.

The opposite of a sugar-bot is not a cold bot.

It is a changing relationship.

One that can warm up.

One that can pull back.

One that can notice how the user behaves.

One where affection is not free just because the user asked for it.

That is the part I think many AI companion products are missing.

---

Disclosure: I used an LLM to help organize parts of this post. The test design, claims, editing, and final responsibility are mine. All quoted transcripts are real bot test outputs; line breaks may be normalized for readability.

Full transcripts:

[Better Models Won't Fix AI Companions](https://github.com/zennos0609-dotcom/ai-companion-realism/blob/main/posts/better-models-wont-fix-ai-companions.md)
