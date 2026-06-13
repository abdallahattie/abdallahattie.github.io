---
title: The Models We Do Not Own
description: Owning the data center is easy. Owning the model that runs on it is the part nobody's guaranteed.
pubDate: 2026-06-13
---
On December 26, 2024, DeepSeek released V3: a 671-billion-parameter model whose technical report put the marginal training run at roughly $5.6 million — not the full program cost, but still a startling figure — with the weights placed on Hugging Face for anyone to download, run, and modify. A month later came R1, and a single day in late January 2025 wiped hundreds of billions off AI-related stocks. Everyone talked about cost, chips, and China. The part that stayed with me was quieter: a frontier-class model had been handed to the world, no permission required.

For about eighteen months, that felt like the direction of travel.

## The argument, in one anecdote

The case for open models isn't that they're cheaper, though they are, or more private, though they can be. It's that you can take them apart. Pinterest is the example I keep returning to. On an earnings call, its CEO told investors they saw "orders of magnitude" cost reduction at comparable performance from fine-tuned open models — a number a CFO has to stand behind. Then their engineers did the thing only open weights allow: they tore the vision encoder out of Qwen3-VL and dropped in their own embeddings. You can't do that to an API. Ownership is the feature.

## The crack — and the counter-crack

Then two anchors moved. In April 2026, Meta launched Muse Spark, its first closed-weight flagship: API only, no download. Days later, Alibaba shipped Qwen3.6-Max with no public weights — the first time in Qwen's history that its best model couldn't be self-hosted, a pattern Qwen 3.7 Max confirmed in May. The two labs that anchored the open side — the Western champion and the most-downloaded family on earth — closed their best work in the same quarter, for the same reason: frontier models cost too much to give away.

I won't oversell this. It is a signal, not a regression line — and the signal cuts both ways. Meta shipped Llama 5 open the *same day* as Muse Spark. Alibaba's open Qwen3.6-27B reportedly beat a 397-billion-parameter predecessor days after the closed Max appeared. Kimi, MiniMax, and DeepSeek remain open. The honest reading isn't "open is dying" but "the frontier is bifurcating" — a closed flagship on top, a strengthening open tier underneath. The question is whether the gap between them widens.

## Why the Gulf should care

I work in the Gulf, and from here the stakes sharpen. The region is committing sovereign-fund money to AI infrastructure at a scale almost no one can match — HUMAIN alone is a roughly $100 billion bet, and regional data-center capacity is set to triple by 2030. I'm broadly for it. A region that wants to matter has to control compute.

But infrastructure is an empty vessel. A gigawatt of GPUs is a means, not an end. If the best models stay closed and API-only, "sovereign AI" becomes a contradiction: you own the building and rent the tenant. Your data-residency story holds right up until the only model good enough lives on someone else's cloud, under someone else's terms, subject to someone else's export regime. We would have spent a hundred billion dollars to become a very well-equipped customer.

And none of this starts from zero. Saudi Arabia's ALLaM, the UAE's Falcon, and Qatar's Fanar are sovereign, Arabic-first models that already lead the Arabic benchmarks — ALLaM nears proprietary systems on reasoning. They are the proof, not the question mark: the region can already build a model it owns end to end, on its own data, in its own language, aligned to its own values. That counts for more than it's usually given credit for. What they don't yet do — and don't claim to — is match the frontier flagships on the broadest, most demanding agentic workloads, where the leading models are an order of magnitude larger. That's not a verdict on the work; it's the distance still to travel. The danger isn't the absence of a starting point. It's mistaking the starting point for the finish line.

## Hedging — for more than supply

So hedge. Not abandon the bet — hedge it, and aim higher than most hedges do.

The reflex is to "secure supply": co-locate a provider's closed model in a local data center so it can't be switched off over the public internet. That's better than an API key, but if it's the whole strategy, we've only built a more expensive cage. Securing supply isn't securing capability.

The Gulf's leverage — hyperscaler-class buildout, sovereign capital — is precisely what you use to negotiate past a customer relationship. Partnerships and investment in model providers should buy three things, not one: operational continuity (multiple providers, contractual portability, weights in escrow where possible); genuine local capability to fine-tune and adapt the models we host; and real skills and knowledge transfer — engineers trained, methods documented, the ability to take the next ALLaM from a strong regional model to a frontier one, not merely to run someone else's. Supply you can lose in a renegotiation. Ownership and know-how you keep.

And keep funding the models that stay open, precisely because they're the only ones we can take apart when we need to.

I meant DeepSeek's giveaway as a hopeful image. Maybe it was the high-water mark; maybe the beginning. I don't know. But "we'll just use the best model when we need it" is no longer safe ground for a hundred billion dollars of infrastructure — and this region, more than most, has the resources to make sure the most important capability it deploys is one it owns.