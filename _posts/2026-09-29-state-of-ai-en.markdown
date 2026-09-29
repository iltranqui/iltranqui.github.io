---
layout: post
discussion: true
title: "State of AI Right Now"
excerpt: "Sonnet 5.5 and Opus 5.5 are out. A plain-language update on what these model releases mean, why intelligence keeps getting cheaper and smaller, and why I'm optimistic."
date:   2026-09-29 10:00:00
lang: en
permalink: /writing/state-of-ai/
alt: /it/writing/stato-dellai/
---

<style>
.post-header h1 {
    font-size: 35px;
}
</style>

Sonnet 5.5 has just come out, and Opus 5.5 came out a few days ago. I know that for a lot of people, these model releases don't mean much in the end, or they simply can't keep up.

What's happening? What are Astra, GPT 6, Luna, Terra? What are all these names that keep popping up: Kimi 3.5, DeepSeek V4.1 Flash? Someone who doesn't follow AI frequently can't keep track of all this. Actually, it all sounds the same to them. I realized this, and I'm writing this blog to update these people, or anyone interested.

## Small steps, and bigger brains

On their own, no single model is an extraordinary leap. It's a small step, a small step in making this technology, LLMs (Large Language Models), a bit smarter. But it's that pinch of extra intelligence that makes them different.

What often happens, for example with the arrival of Mythos on June 1st, and then Fable 5, is that this class of enormous models was born. For those who don't know, these models literally have a "size," as if they were 100 billion, a trillion, two trillion, five trillion or 10 trillion parameters, whatever it is. What was noticed in training these big models, which in the end just predict the most probable next word after a sentence, is that they keep getting bigger. And a principle known as [The Bitter Lesson](http://www.incompleteideas.net/IncIdeas/BitterLesson.html), by Rich Sutton, showed that, instead of doing fancy, clever tricks, these models somehow just become smarter, unlocking abilities we still can't fully explain, simply by making them bigger. Like a brain that is, in quotes, "more connected," which means it's able to understand more things.

But how do you tell the difference in intelligence between these models? As a programmer, when I have tasks to complete, moving from a smaller model, with a smaller brain, to a bigger one, I notice it's literally better at understanding my intent, understanding what I want to do, and moving forward. And not only that.

For example, with Haiku 4.5, you give it a task and it gets lost fairly quickly. Now with Sonnet 5 it can do more, though in some contexts things still get difficult. Going up to Opus and even Fable, you increasingly get the impression of talking to a person who not only understands better what you want to do and communicate, but who also, the longer you work with them, keeps in mind for longer what you told them earlier.

And the amazing thing being noticed is that these models are getting smart at ever smaller sizes. The intelligence capable of finely understanding things used to be confined to bigger models. Now that seems to be shrinking. So we have a model with a 5-trillion brain (I'm throwing out fairly random numbers here), and the same intelligence in a one-trillion model, and even lower.

The more this technology moves forward, the more evident it becomes that the ability to embed intelligence, the ability to understand what a person wants these programs to do, is becoming more and more compact. And that's a good thing, because with even simpler tools, lots of small tasks can be carried out for even longer.

## What does this mean for people?

Enrico, there's this AI bubble, what's going on? Everything. I see that this technology isn't going away. Say Anthropic and OpenAI literally fail spectacularly, they collapse, everything is lost, and so on. It's not like the models go poof and disappear. They'd go to someone else, someone else would absorb them, whether Microsoft or Amazon, or they'd be broken up and spread elsewhere, or maybe it wouldn't even happen.

But the point remains that intelligence is getting cheaper and more portable. We're pushing to reduce the costs of all this, but at the same time we're also pushing to make models bigger. Why? First of all, it's great to have a PhD-level brain, as many of these labs say, in your pocket, on your phone. I make a request, tell it a story, and it can go find exactly what I want somewhere.

But at the same time, these models are becoming more capable of interacting with the world. For example, GPT 6 Astra has been seen navigating a computer: opening a window, opening a browser, placing an order or making an online booking, whatever it may be. And beyond words, where they can write poems, do scientific research, and see paths we humans can't keep in mind, they're also starting to genuinely understand what's in images.

And yes, they have all the data of the internet inside them, but what's being understood more and more is that the more data you give them, the better they understand in some way. It's not that they give you the right answer. Many people say, "But I ask ChatGPT or Anthropic something, and then it says, 'Ah yes, you were right here.'"

This is because so many people, in my opinion, get the approach to this technology wrong. Most people, I think, approach this as a program. Many people see it as just a program and expect: I tell a program to do this thing. Say they look up the names of the four Beatles, and, depending on whether a model is dumber or smarter, one gives you the right answer and another might give you the wrong one, because they have this thing called hallucination. Hallucination, as many would say, is both a bug of the algorithm used and a feature, because it's exactly what allows them not only to say wrong things, but also, in some cases, to do something new that you don't expect. They become good at writing a program that resembles many things they've seen, but in this case even better. It's part of progress, and it's exactly this thing that annoys most people so much.

I'm not saying people don't understand this technology, but if you understand well how it reasons, how it thinks, then you know how to interact with it.

## Why code and math are "solved" first

As a programmer, the nice thing is that I can always verify the work. If I write a program and tell the computer to do something, the computer can tell me: "Look, no Enrico, this doesn't work, because in this line of code you wrote there's an error." So I get feedback from that standpoint. LLMs have improved enormously at writing code and becoming excellent programmers, and also at math. Why? Because they can get immediate but also accurate feedback, since the result is, in quotes, "deterministic."

If I write a program and tell the computer, "No, I want to do this," it's an error, I fix that, I write something else, another error... in the end, with the computer's help, the compiler's help, I can compile the program and see that it works. The same holds in many languages and in math, so I can tell the LLM: "Train on all this data," because I can give it feedback that's also accurate, also correct. That's why math and programming have become dragons (i.e., they're mastered): I either succeed or I don't. When I succeed, good. When I don't, the computer itself tells me there's an error somewhere.

And since the LLM can reason at millisecond speeds, or at least very fast, it can try 100 things in a minute, while we humans try one thing a minute. That's why they're dragons at reasoning about code, math, and all these things.

All of this is to say that if I can verify my output, I can do it, as long as the result is verifiable in a short time. Say I have 100,000 rules to respect, in code or whatever. I tell it: "Write the code until all of these things are satisfied." The LLM writes the code, one rule at a time, so as to satisfy them all. That's why they're brilliant.

But there's no deterministic way to say "this apple is good," because that's subjective. It's not something like "this person likes it, this person doesn't." So in that case, what do LLMs do? They just guess.

So I see that these tools will be brilliant at automating all the processes that are finite, logical and deterministic. And honestly, doing mechanical work, entering data on the computer, I personally think it's a waste of people's time in this world to do repetitive things on a computer. Sure, there may be someone who enjoys it, but in that case it'll go against those people.

## Where I think this is going

That said, in my opinion the first predictions from now on are these: these models will become smarter and better, at lower cost and smaller size, despite the whole AI economy bubble. It's a bit inflated right now because obviously these people want to make money and get rich. But I don't think this technology is going away.

Also worth noting: models are defined by their weights. Once I have them, they won't become dumber in the future. If I develop a program and the new version is dumber, I won't ship it, I'll keep what I already have. Models keep becoming smarter, more capable, able to do more abstract things, or cheaper, or both.

One thing being developed now is ways to reduce the cost of this technology to make it more local, more reliable, and usable by more people. At the same time, there's a push to make these programs bigger in order to abstract more. It's what has always happened with programming languages: from Assembly to C, to C++, to Rust, to Python. What you do, and what you want, is to keep abstracting thought, or make the problem "bigger." What do I mean by bigger? Instead of "move this bit to that bit... wait, computer, I want you to do this, then take this from here and move it there," those are the low-level instructions. The further we go, the more we'll be able to literally explain what we'd like to these models, and they'll be able to do it.

Now the big models are also getting good at understanding images. There may be a limit at some point, but we'll find a way to make them understand images, and in the future video. In the future, it could literally be that I don't give the prompt to the LLM, I give the video to the LLM, and in the video I show it: "Look, there's this thing here, and this thing here. Could you explain it better, or do whatever?"

So the ability to express the problem I want these machines to solve will become greater, more reliable, and simpler to use. Also because there's an infinite number of problems to solve: for anyone who has worked in a company, or just looks around, there are plenty of problems that, with a bit of ingenuity, could be somewhat automated. Maybe I'm saying this from a bias, since I studied automation engineering at Politecnico di Milano, both bachelor's and master's. It could be a bias, but so be it.

So I always see this technology as a positive thing, because now we can do more in less time, and make it robust too. I go against the idea that these technologies are "oh my god, they hacked something, oh my god, they escaped." Folks, these programs are programs. It's like on/off: I turn them on, I turn them off, and not only that, I also tell them what to do. And if they do these things, it's because they were told to. When I search for a bug in cybersecurity, it's me telling it "look for a bug in this binary or somewhere else." They aren't dangerous in themselves. The people who use them are the dangerous ones.

It's also true that they're evolving at a pace we literally can't keep up with. At the time of this article, Sonnet 5.5 has been out for an hour and a half. I'm sure that in less than a month the Chinese models, whether Kimi, DeepSeek, Zhipu, or something else, will release a model that's more powerful or cheaper, we don't know which. But it's the small sum of all these things that will make this industry grow, and it keeps going and going.

It moves forward. I like this technology because it lets you do so many things, and that's the beautiful, fun part, because a lot of people are using it to create things. I now have an idea in my head, and I can make it real. Before, I had to figure out how to move a bit here and there; now I describe what I want, it understands me and modifies exactly what I want. That's the wonderful thing, because now I'm no longer limited by "oh my god, this idea will take me 20 hours." Now I can just describe it and it does it. Whether it's robust, works every time, has no bugs, and is fully secure is another question. But the ability to have an idea in my head and tell it to a program, and have it come out very close to what I had in mind, I find that absurd and absolutely phenomenal.

As a YouTuber says: what a time to be alive!
