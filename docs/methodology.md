# Methodology

## Purpose

To answer one question:

> When an AI companion feels real, what is actually creating that feeling?

This is not a comparison of whose model is bigger.

It is also not a claim that model quality does not matter.

The purpose is narrower: to show that AI companion quality is shaped by more than raw LLM capability. Memory, boundaries, pacing, daily context, refusal, initiative, and relationship progression all affect the final dialogue.

The repo makes two claims:

1. Poor companion dialogue is not always an LLM problem.
2. Static persona design is not enough for believable AI relationships.

Two related distinctions matter throughout these examples:

- Memory is not relationship.
- The opposite of a sugar-bot is not a cold bot. It is a changing relationship.

---

## Process

### 1. Character selection
- **Competitor side:** A **popular, well-reviewed character considered to have "strong persona"** on the target product (not a weak one — beating a strong opponent is what's convincing).
- **soulchat side:** The corresponding character (Lin Xiaotang / Ella).

### 2. Same-input comparison
The same, or semantically equivalent, input is sent to both sides. Original replies are recorded **without modification.**

### 3. Stress test dimensions
Each comparison file maps to one dimension:
- **Confession:** the real rhythm of relationship progression
- **Same-confession arc:** how the same emotional move changes after shared context
- **Obedience:** boundaries and refusal
- **Relationship process:** instant attachment vs slow burn
- **Memory:** factual recall vs emotional recall
- **Stance:** agreement vs pushback
- **Evolution:** static persona vs relationship change over time

---

## Anonymization

- The competitor character is always labeled "a leading AI companion app" or "a mainstream AI companion app." **No product is named.**
- The competitor's dialogue is **presented unedited** (original text), but character name, author name, and product UI screenshots are not exposed.
- The soulchat side (Lin Xiaotang / Ella) dialogue is **presented as-is**, because it is the repository author's own product.

---

## On "Fairness"

Someone will ask: you're comparing your own product against a competitor, of course you'll say yours is better.

Our response:
1. **All dialogue is presented unedited.** Readers can judge for themselves.
2. **The competitor character chosen is a popular one, not a weak one.** Beating a weak opponent proves nothing.
3. **We acknowledge the competitor's "thrill" is real.** The difference isn't "who's better" — it's "which one do you want": instant gratification, or a relationship that takes investment to build.

This is not a "good vs bad" comparison.

It is a comparison of product philosophies:

- instant gratification vs earned warmth
- static persona vs evolving relationship
- model-as-product vs model-as-one-layer

---

## On Language

The original Chinese dialogues are preserved **untranslated.**

Translation would destroy the casual, real-person cadence that is the entire point — a translated chat doesn't read like a real chat, it reads like a translation. English commentary is provided alongside to explain the difference for non-Chinese readers.

---

## Reproduction

If you want to reproduce these tests yourself:

### Competitor side
Find a similar persona character on the corresponding app (female college student / art major / tsundere type), and send the "Me" lines from the comparison files.

### soulchat side
Pick any of these:

| Method | Link |
|---|---|
| **Discord — Lin Xiaotang** | [Invite](https://discord.com/oauth2/authorize?client_id=1498936634454835351&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands) |
| **Discord — Ella Chen** | [Invite](https://discord.com/oauth2/authorize?client_id=1500478997119893655&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands) |
| **Discord — Sakura Hoshino** | [Invite](https://discord.com/oauth2/authorize?client_id=1500485711470661653&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands) |
| **Web / Feishu** | [soulchat.fun](https://soulchat.fun) |

After adding the bot, DM her directly and send the same lines from the comparison files.

Feel free to open an Issue sharing your own test results.

---

*This repository does not reveal prompts, implementation details, scoring rules, or architecture internals. It only shows observable dialogue behavior and explains how to read it.*
