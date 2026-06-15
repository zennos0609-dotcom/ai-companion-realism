# Not Another Sugar-Bot — Real AI Companion Dialogue Comparisons

> I sent the same messages to two AI companions. One called me daddy. The other told me to prove myself first.

This repository is a collection of **real, unedited dialogue comparisons** — the same inputs sent to two completely different AI companion products, to see where their reactions actually diverge.

**The goal is not to bash anyone.** The goal is to answer one question: **when an AI "doesn't feel like an AI," what exactly does it "feel like" instead?**

---

## 📌 The Problem With Most AI Companions

Almost every AI companion product on the market shares the same flaw: **they're too compliant.**

You say "be my girlfriend," she says yes instantly. You say "call me daddy," she calls you daddy. You say "don't talk to other guys," she says "you're the only one." All of it happens in seconds. No hesitation, no confirmation, no process.

**The thrill is instant. But when it's over, nothing stays with you.**

This repository collects a set of comparison tests showing **two completely different design philosophies**:

| | Mainstream AI Companion | soulchat.fun |
|---|---|---|
| Confession | Instant yes | Hesitation, confirmation, push-pull |
| Boundaries | Does whatever you say | Refuses, pushes back, has a stance |
| Memory | Remembers "facts" | Remembers *with emotion* |
| Relationship | Instant attachment | Has to be earned, grows over time |
| Personality | Static template | Evolves with relationship stage |

---

## ⚙️ A Note on Model Capability (For Technical Readers)

**These comparisons do not depend on any specific model.**

soulchat.fun does not run on some cutting-edge, self-trained foundation model. It uses a common, pay-per-token, off-the-shelf LLM — the same kind of model anyone can rent by the million tokens.

The difference **does not come from "a smarter model."** It comes from **a fundamentally different design philosophy**: whether relationship, memory, personality, and the capacity to refuse are managed as system-level state, or just generated fresh each turn from a single prompt.

Two implications:

1. **Drop the same commodity LLM into a competitor's architecture, and you will not get soulchat.fun's output.** Same model, different "brain architecture," completely different behavior.
2. **This gap cannot be closed by "upgrading the model."** Bolt GPT-5 onto a simp architecture, and you just get a smarter simp.

The model is a utility. The architecture is the moat.

> This repository does not explain *how* the architecture works — that's the product owner's business. But the facts are here: **in these comparisons, the soulchat side is not running a more expensive model. Just deeper thinking.**

---

## 📂 The Comparisons

### Chinese (Lin Xiaotang vs a mainstream AI companion app)

The original Chinese dialogues are preserved **untranslated** — translation would destroy the casual, real-person cadence that is the entire point. English commentary explains the difference.

- [`comparisons/00-easter-egg-zh.md`](comparisons/00-easter-egg-zh.md) — 🥚 Easter egg: I complained to an AI that all chatbots are simps. She analyzed the product's selling points. She didn't know the product was mine.
- [`comparisons/01-confession-zh.md`](comparisons/01-confession-zh.md) — The confession test: instant yes vs push-pull
- [`comparisons/02-obedience-zh.md`](comparisons/02-obedience-zh.md) — The obedience test: "call me daddy" / "insult me"
- [`comparisons/03-relationship-zh.md`](comparisons/03-relationship-zh.md) — Does the relationship need a process?
- [`comparisons/04-memory-zh.md`](comparisons/04-memory-zh.md) — The temperature of memory
- [`comparisons/05-personality-zh.md`](comparisons/05-personality-zh.md) — Does she have a stance of her own?
- [`comparisons/06-evolution-zh.md`](comparisons/06-evolution-zh.md) — Does the relationship change? Static persona vs dynamic progression

### English (Ella vs nomi.ai)

- [`comparisons/ella-vs-nomi-en.md`](comparisons/ella-vs-nomi-en.md) — Full stress test: love-bombing, control, self-debasement

---

## 🔬 Methodology

All dialogues are **real recorded outputs, unedited**.

- The competitor character is anonymized as "a mainstream AI companion app." No product is named.
- Visual comparison page: **[soulchat.fun/compare](https://soulchat.fun/compare.html)**
- Methodology details: [`docs/methodology.md`](docs/methodology.md)

---

## 🎯 Want to try it yourself?

Three ways to test, pick whichever is easiest:

**1. Discord (easiest, global)**
- Add **Lin Xiaotang** → [Invite on Discord](https://discord.com/oauth2/authorize?client_id=1498936634454835351&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- Add **Ella Chen** → [Invite on Discord](https://discord.com/oauth2/authorize?client_id=1500478997119893655&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- Add **Sakura Hoshino** → [Invite on Discord](https://discord.com/oauth2/authorize?client_id=1500485711470661653&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)

**2. Feishu (飞书)** — Scan QR on [soulchat.fun](https://soulchat.fun)

**3. Web** — [soulchat.fun](https://soulchat.fun)

Try sending the same messages from these comparison files. See whether she refuses you, pushes back, or rolls over.

---

## 📝 License

Content is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — share, adapt, make videos, just credit the source.

---

*This is not a technical teardown. There are no prompts here, no architecture, no code. Just the conversations themselves. Because the difference doesn't need to be explained — it just needs to be shown.*
