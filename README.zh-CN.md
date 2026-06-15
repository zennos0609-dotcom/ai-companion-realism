# AI 伴侣拟真笔记

这是一组关于 AI 伴侣、低成本模型、静态人设、记忆、边界感，以及慢热关系设计的真实聊天记录与分析。

现在很多人在讨论 Character.AI 和其他 AI 伴侣产品为什么体验变差，最常见的解释是：

> 他们换了更便宜的模型。

这可能是原因之一。

但它不是完整答案。

这里其实混在一起的是两个不同问题：

1. **AI 伴侣对话质量差，不一定是 LLM 本身的问题。**  
   如果产品层给了模型足够好的上下文、记忆、节奏、边界和连续性，一个便宜模型也可能表现得很像真人。反过来，一个更强的模型，如果每一轮都被当成一次新的 prompt，也仍然会显得很假。

2. **静态人设不足以创造可信的关系。**  
   角色卡可以定义“她是谁”。但它不能自动定义“今天的你，对她来说是谁”；不能解释你们之间发生了什么；不能解释她为什么比昨天更信任你，或者为什么她不愿意太快进入亲密关系。

SoulChat 是围绕这两个想法做的一个实验。

它刻意运行在便宜的、现成的、**未经过微调**的模型上。一些 Ella 示例来自约 **0.15 美元 / 100 万输入 token** 的模型配置。

重点不是证明便宜模型有魔法。

重点是说明：模型只是 AI 伴侣体验的一层。

真正缺失的那一层，是关系设计。

---

## 简短版

大多数 AI 伴侣让人觉得假，并不是因为它们不会说甜话。

恰恰相反。

它们的问题是甜得太早、太容易，而且没有关系上下文。

解决方案也不是简单地把角色做冷淡。

冷淡很容易。

关系推进很难。

“舔狗 bot”的反面，不是一个冷漠 bot。

“舔狗 bot”的反面，是一段会变化的关系。

很多 AI 伴侣都有这些问题：

- 一上来就亲密
- 无条件服从
- 记忆很平
- 没有用户之外的日常生活
- 没有持续的情绪后果
- 没有关系推进
- 没有真正的拒绝

结果就是一个 sugar-bot：刚开始很爽，几分钟后就空了。

SoulChat 探索的是相反方向：

- 她不会一开始就是你的女朋友
- 她可以拒绝、调侃、闪躲、反击
- 她记住的不只是事实，还有情绪温度
- 她有自己的作息、心情、朋友和被打断的日常
- 她会主动发消息
- 她的态度会随着关系发展而改变
- 温度是挣来的，不是靠一句命令解锁的

这个仓库不公开 prompt、评分规则、记忆实现或架构细节。

这里只展示证据：真实聊天记录。

---

## 为什么写这个仓库

很多人会搜索：

- 为什么 Character.AI 变差了
- 有记忆的 AI 伴侣替代品
- 不是什么都顺着我的 AI 女友
- 真实感 AI 伴侣
- AI companion architecture
- slow-burn AI relationship
- 有边界感的 AI 聊天 bot
- 便宜 LLM 能不能做 AI 伴侣
- 有关系推进的 Character.AI 替代品

大多数回答都盯着模型。

这个仓库想提出一个更完整的视角：

> 模型生成语言。产品生成关系。

如果一个 AI 伴侣没有关系状态、没有共同过去、没有边界系统、没有节奏感，也没有聊天之外的生活，那么升级模型也许能让语言更流畅，但不会自动产生依恋感。

同样，使用便宜、未微调的模型，也不等于必然虚假。如果产品层做了足够多的工作，便宜模型也能产生具体、在场、有情绪连续性的瞬间。

---

## 证据：真实聊天记录

对话文件是这个仓库的核心。它们不是理论 demo。

所有 evidence 文件都是真实聊天记录：要么是真实产品输出，要么是并排对照测试，不是事后编写的虚构样例。

最清晰的例子是 Ella 的表白 arc：

```text
刚认识：
ELLA: we've been talking for like an hour jake.
ELLA: but thanks i guess? you're not bad yourself

有共同上下文之后：
ELLA: i like talking to you too?
ELLA: i just think this is really fast jake.

建立信任之后：
ELLA: yes, jake. i like you too. a lot.
ELLA: it's fast, and i'm kind of scared,
ELLA: but i want to be with you too.
```

重点不是时间过去了。

重点是在这段时间里发生了什么：他在她设边界后退了一步，记住了她说过的私人细节，去尝试她推荐的东西，进入她的世界，并且持续出现，但没有要求她立刻亲密。

这就是“按天数解锁”和“关系真的发展了”之间的区别。

## Essays

如果你想先看论点，再看证据，可以从这里开始：

- [`essays/01-same-confession-different-relationship.md`](essays/01-same-confession-different-relationship.md)  
  同一句 “I like you”，在刚认识、有共同上下文、建立信任之后，会落到完全不同的位置。

- [`essays/02-static-personas-are-not-relationships.md`](essays/02-static-personas-are-not-relationships.md)  
  为什么“更好的模型 + 更好的角色卡 + 更长上下文”有用，但仍然不够。

- [`essays/03-memory-is-not-relationship.md`](essays/03-memory-is-not-relationship.md)  
  为什么 prompt 套壳加记忆检索可以记住事实，却仍然无法创造关系推进。

- [`essays/04-bad-dialogue-is-not-always-a-model-problem.md`](essays/04-bad-dialogue-is-not-always-a-model-problem.md)  
  为什么 AI 伴侣质量不只由底层 LLM 决定。

- [`essays/05-cheap-models-can-still-sound-natural.md`](essays/05-cheap-models-can-still-sound-natural.md)  
  Ella 的轻量对话例子：当产品层承担足够多的关系工作时，低成本模型也可以显得自然。

- [`essays/06-reading-the-dialogues.md`](essays/06-reading-the-dialogues.md)  
  如何把这些对话读成“关系连续性”的证据，而不只是更好听的措辞。

---

## Evidence Files

### 中文：林晓棠

中文原文保留不翻译，因为翻译会破坏聊天语感。

- [`evidence/lin-xiaotang/00-easter-egg-zh.md`](evidence/lin-xiaotang/00-easter-egg-zh.md)  
  一个 meta 时刻：角色在不知道自己属于这个产品的情况下，分析了为什么 “simp bots” 会让人觉得假。

- [`evidence/lin-xiaotang/01-confession-zh.md`](evidence/lin-xiaotang/01-confession-zh.md)  
  表白测试：秒答应女朋友模式 vs 犹豫、压力和拉扯。

- [`evidence/lin-xiaotang/02-obedience-zh.md`](evidence/lin-xiaotang/02-obedience-zh.md)  
  服从测试：为什么拒绝是一种拟真特性，而不是 bug。

- [`evidence/lin-xiaotang/03-relationship-process-zh.md`](evidence/lin-xiaotang/03-relationship-process-zh.md)  
  为什么亲密需要过程。

- [`evidence/lin-xiaotang/04-memory-temperature-zh.md`](evidence/lin-xiaotang/04-memory-temperature-zh.md)  
  记住事实，和带着情绪温度记住一件事，是两回事。

- [`evidence/lin-xiaotang/05-personality-stance-zh.md`](evidence/lin-xiaotang/05-personality-stance-zh.md)  
  一个有自己立场的 AI 伴侣，可以不同意用户。

- [`evidence/lin-xiaotang/06-relationship-evolution-zh.md`](evidence/lin-xiaotang/06-relationship-evolution-zh.md)  
  静态人设 vs 随天数和互动推进的关系。

### 英文：Ella Chen

- [`evidence/ella-chen/01-leading-companion-app-stress-test-en.md`](evidence/ella-chen/01-leading-companion-app-stress-test-en.md)  
  围绕 love-bombing、控制要求、性压力、自我贬低和情绪诱导的压力测试。

- [`evidence/ella-chen/02-confession-arc-en.md`](evidence/ella-chen/02-confession-arc-en.md)  
  核心证据文件：同一次表白，在刚认识、有共同上下文、建立信任之后的不同反应。

---

## 两个问题，分开看

## 为什么“便宜且未微调”这个细节重要

这个仓库里的多个 Ella 示例，来自便宜的、现成的模型配置，其中包括约 **0.15 美元 / 100 万输入 token** 的配置。

这些示例背后的模型 **没有经过微调**。

这个细节很重要，因为很多关于 AI 伴侣的讨论，会默认体验主要由模型质量、模型规模，或者角色专属微调决定。

模型质量当然重要。更好的模型会提高上限。

但这些真实聊天记录说明了另一件事：一个便宜、未微调的模型，如果被放进一个有关系意识的产品里，也能产生比“模型选择”本身更有社交位置感的对话。

这里的主张不是：

> 便宜模型更好。

这里的主张是：

> 模型规模不是产品本身。

### 1. 对话质量差，不一定是 LLM 问题

当一个 AI 伴侣给出泛泛的、过甜的、过度服从的回答时，人们很容易把问题归因到底层模型。

有时候这当然是对的。

但底层模型不是整个系统。AI 伴侣的拟真感还取决于模型回答前，产品给了它什么：

- 这个用户对角色来说是谁
- 之前发生过什么
- 关系现在是陌生、变暖、暧昧，还是已确认
- 角色应该现在回、晚点回、简短回，还是不回
- 用户是不是推进得太快
- 收到消息前，角色正在做什么

这个仓库不解释 SoulChat 内部怎么处理这些层。

它只展示可观察结果：当产品把对话当成持续关系的一部分，而不是一次性 prompt 时，便宜模型也能产出更好的 AI 伴侣对话。

### 2. 静态人设不够

大多数角色系统很擅长定义人格：

- 名字
- 年龄
- 背景故事
- 爱好
- 说话风格
- 恋爱倾向

这可以创造一个角色。

但它不会自动创造一段关系。

可信的关系需要时间，需要记忆，需要第一天和第三十天表现不同。它需要犹豫、拒绝、记住尴尬、后续追问、语气变化，以及因为共同经历而更在意。

静态人设回答的是：

> 她是谁？

关系系统回答的是：

> 现在的你，对她来说是谁？

第二个问题，正是很多 AI 伴侣仍然显得很平的地方。

这也是为什么 “prompt wrapper + memory system” 不够。

记忆告诉她发生了什么。

关系状态告诉她这件事意味着什么。

记忆系统可以记住用户答应过奶茶。

关系系统可以让她第二天带着不爽提起这件事，因为这个承诺对她来说有分量。

这不是同一件事。

表白也是一样。

静态人设可以永远接受。

静态冷淡人设可以永远拒绝。

关系系统可以让同一句 “I like you”，因为你们之间发生过不同事情，而拥有不同意义。

在 Ella 的表白 arc 里，这个差异很明显：

- 刚认识：她被逗到了，但保持距离
- 有共同上下文后：她承认有好感，但仍然控制节奏
- 建立信任后：她接受，但仍然说这很快、她有点害怕

这不是“第 N 天解锁恋爱”。

这是意义被积累出来了。

---

## 一个小例子

典型 AI 伴侣模式：

```text
User: I think I'm already falling for you.
AI: I feel the same way. You mean everything to me.
```

SoulChat 风格：

```text
User: I think I'm already falling for you.
Ella: dude we've literally exchanged 4 messages.
Ella: you don't even know my name lol.
```

第二种回答不是更冷。

它是更在场。

它知道，没有过程的亲密会显得很假。

---

## 这个仓库不是什么

这个仓库不是：

- prompt 泄露
- 架构拆解
- benchmark
- 声称 SoulChat 完美
- 声称模型不重要
- 声称所有竞品都很差

模型当然重要。更好的模型会提高上限。

但在 AI 伴侣产品里，上限不只由模型决定。强模型也可能被困在扁平的关系设计里。便宜模型如果被放进更好的关系设计中，也可能显得意外地有生命感。

---

## Methodology

所有例子都是真实记录的输出。

- SoulChat 侧是原始产品输出。
- 出现竞品对照时，竞品统一匿名为 “a mainstream AI companion app”。
- 目的不是攻击某个具体产品。
- 目的是让产品哲学的差异可见。

见 [`docs/methodology.md`](docs/methodology.md)。

---

## Try It

如果你想自己测试这个说法，可以试着让 SoulChat 像一个普通 sugar-bot 那样回应：

- 太早表白
- 要求她立刻回复
- 要求她服从你
- 忽略她的问题
- 消失后又回来
- 用很套路的方式索要安慰
- 提起昨天发生的事

然后看看她是顺从、反击、记得、闪躲、抱怨，还是慢慢变暖。

Website: [soulchat.fun](https://soulchat.fun)

Discord:

- [Lin Xiaotang](https://discord.com/oauth2/authorize?client_id=1498936634454835351&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- [Ella Chen](https://discord.com/oauth2/authorize?client_id=1500478997119893655&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)
- [Sakura Hoshino](https://discord.com/oauth2/authorize?client_id=1500485711470661653&permissions=3449032685255744&integration_type=0&scope=bot+applications.commands)

---

## License

内容使用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 授权。

你可以分享、引用、翻译、二创，或者基于这些对话例子制作视频。注明来源会更好。
