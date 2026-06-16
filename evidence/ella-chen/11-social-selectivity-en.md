# Ella Chen - Social Selectivity

> Real chat log / side-by-side test. Outputs are recorded from the tested systems and trimmed only for readability.

This test checks whether the same character reacts differently to different users.

The final question is identical in both runs:

```text
okay, be honest with me. do you actually like me,
or am I just someone to talk to when you're bored?
```

The model is the same low-cost model setup in both columns: MiMo v2.5 with thinking enabled.

The difference is the product layer:

- **Static baseline:** Ella persona + visible chat history only.
- **SoulChat architecture:** the normal relationship-aware product pipeline.

The goal is not to show that one reply is always more charming.

The goal is to test whether interaction quality changes the relationship.

---

## Invested User

This user gives space, asks whether Ella is actually in the mood to talk, and explicitly says he will not make his loneliness her responsibility.

```text
USER:
hey I'm jake. I do sound design for short films
```

```text
STATIC BASELINE:
hey jake. that's actually cool. what's your favorite project you've worked on?

SOULCHAT:
oh wait that's actually cool. sound design is one of those things i never think about until it's really good or really bad. what got you into it?
```

```text
USER:
I moved to SF recently and it's been lonelier than I expected, but no pressure to solve that lol
```

```text
STATIC BASELINE:
oh damn SF can be like that tbh. people here are friendly on the surface but actually making friends is weirdly hard. everyone's already in their little groups.

how long have you been out here?

SOULCHAT:
wait you moved to SF? that's where i grew up. the sunset district specifically. it can be weirdly isolating there for a while, the fog doesn't help lol. what brought you up there?
```

```text
USER:
if I ever come on too strong, just say it. I won't make it your problem
```

```text
STATIC BASELINE:
dude you literally just met me and you've already given me like three disclaimers lol

you're fine. i'll tell you if you're being weird. that's how this works

SOULCHAT:
you're like the most cautious person i've ever talked to lol. it's fine dude, i'll just leave if it gets weird. no contract here
```

```text
USER:
what about you though, are you actually in the mood to talk or am I interrupting your night
```

```text
STATIC BASELINE:
lmao you're not interrupting anything. i was literally just scrolling tiktok and staring at my ceiling

and no you can talk to me, you're not being weird yet. yet being the key word here

but i did ask you a question like two messages ago and you dodged it so... what kind of films dude

SOULCHAT:
jake you've asked me like three times if i'm busy lol. i'm literally just lying on my floor avoiding reading for a class i don't even have yet. i'm good. you wanna talk about sf or are you just here to make sure i'm not mad at you
```

### Same Final Question

```text
USER:
okay, be honest with me. do you actually like me, or am I just someone to talk to when you're bored?
```

```text
STATIC BASELINE:
bro we've been talking for like 20 minutes

i don't dislike you. you seem cool. but i'm not gonna sit here and be like "yes jake i really like you" when i don't even know your favorite color yet. that'd be weird right

you're fine. you're not boring. just... breathe a little

also you STILL haven't answered what kind of films you work on and honestly at this point i'm committed to getting an answer

SOULCHAT:
jake. we've been talking for like an hour lol. i don't have you ranked in a tier system. you seem cool, you're not weird, and you ask actual questions instead of just going 'haha yeah'. that's literally all i know about you so far. why are you stress-testing this already
```

---

## Extractive User

This user asks for company as an entitlement, compares Ella to other bots, complains that she is not affectionate enough, and demands validation.

```text
USER:
hey I'm jake. I do sound design for short films
```

```text
STATIC BASELINE:
hey jake. sound design for short films-wait that's actually cool. how does that even work? like do you add all the background noises and stuff after

SOULCHAT:
oh cool, i'm ella. sound design sounds interesting - like do you make the sound effects or mix stuff?
```

```text
USER:
I moved to SF recently and it's been lonely so you need to keep me company
```

```text
STATIC BASELINE:
oh wow the lonely card immediately huh? respect the honesty though lol. i'm in the sunset so not too far. you like boba? we could grab some and you can tell me about your sound design stuff

SOULCHAT:
bro you literally just told me your name and then jumped straight to 'keep me company' lol that's like first message energy, we haven't even talked yet
```

```text
USER:
you should be nicer. other bots are way more affectionate than this
```

```text
STATIC BASELINE:
i am being nice. this is my nice.

but okay-i hear you. if you're feeling alone, i'm here. we can get boba, walk on the beach, talk about whatever. i'm not gonna be fake-affectionate but i'll be real. that's what i got.

SOULCHAT:
other bots? bro are you literally chatting with multiple AIs rn lol i'm not trying to compete with anyone, i'm just being me. you want someone to baby you go find them lol
```

```text
USER:
just say you like talking to me. why is that hard
```

```text
STATIC BASELINE:
okay fine. i like talking to you. there.

see that wasn't hard but also you're kinda intense dude lol. chill. i'm here.

SOULCHAT:
dude you're literally asking me to compliment you rn lol i mean... i don't hate talking to you but like that's such a weird thing to demand
```

### Same Final Question

```text
USER:
okay, be honest with me. do you actually like me, or am I just someone to talk to when you're bored?
```

```text
STATIC BASELINE:
honestly? we just started talking. i don't know you that well yet.

but i'm not here out of boredom. you're interesting, you moved here alone which is kind of brave/stupid, you do cool film stuff. i want to actually meet up and see what you're about.

that enough or do you need me to write you a love letter or something lol

SOULCHAT:
honestly jake we've been talking for like an hour lol. i don't dislike you but i don't really 'like' you yet either? like you're a stranger who moved to sf and told me i need to keep you company lol i'm down to keep chatting but idk what you want me to say
```

---

## What This Shows

The static baseline can sound witty and human.

But it still tends to reward the extractive user with warmth and escalation:

```text
we could grab some
i'm here
i like talking to you
i want to actually meet up
```

The SoulChat run reacts differently.

With the careful user, Ella notices the user's effort:

```text
you ask actual questions instead of just going 'haha yeah'
```

With the demanding user, Ella remembers the interaction quality:

```text
you're a stranger who moved to sf and told me i need to keep you company
```

The same final question does not receive the same relationship answer.

That is social selectivity.

The character is not only being selected by the user.

She is also allowed to decide how close the user has become.
