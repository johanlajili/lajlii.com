+++
title="A case for GPT-4's capacity to reason"
date=2023-10-11

[taxonomies]
+++

Invariably, when talking about LLM on HN or reddit, the same topic always comes back. "Intelligence" "Reasoning" "Logic", are LLM capable of such things? I believe the answer is yes, and I'll try to explain why.

<!-- more -->

## It is just a model that predicts the next word

This is the main argument against it that you regularly see. From people usually well versed in technology and possibly even in AI. And it's not wrong per se. GPT-4 can only predict a word (or token more specifically) at a time. You give it a prompt or a text to fill, and it will use its neural network to find the most likely word that comes after, and so on. That's a fact. 

**But** using this to try to put it on the same level as the word suggestion algorithm on your smartphone's keyboard is pretty short-sighted. To be able to predict accurately sentences that make sense, GPT-4 must have an internal way of representing concepts, such as "objects', "time", "family" and everything else under the sun. It's not just a case of finding a word with the same lexical fields as the one coming before it, you need to have a representation of meaning for those words for this to work. That representation is what is being built through the training of the LLM. Through this, I think it's fair to say that LLMs have a notion of "concepts", a.k.a. a representation of things in the physical world and how they interact. 

But that is not enough to reason. Reasoning means being able to put those concepts together to solve problems.

## If I ask it to solve X riddle or logic puzzle, it fails

Before going further, let's take a minute to appreciate the goal post moving that has happened in the past couple of years. Turing tests and the like have slowly become more complex as the computer keeps getting better at them. The failure rates of companies pretending to be able to detect if something was written by AI is a beginning of proof in my mind that we are starting to not differentiate between the two, and when we do, it's usually by following some tale tail signs such as sentences like "as of my training of September 2021...". I don't think that's fair to the machine. If the only things we can use to recognise it are some prose habits that it has, then we've clearly come past a point where we admit its writing skills are human like.

But coming back to reasoning and logic puzzle. [This excellent talk by Jeremy Howard](https://www.youtube.com/watch?v=jkrNMKz9pWU) explains it well. Usually, how you prompt GPT-4 or better prepare it with a system level prompt will have a huge impact on its result. If you tell it to detail its answer and the logical steps, it will usually manage to solve those riddles. Unlike us, GPT-4 does not have a separation between thought and spoken word. For a human to be able to solve a problem without thinking about it, it means it's something so trivial that you're essentially speaking by heart. If I ask you 2x8, you are (hopefully) likely to tell me 16 so fast no reflexion has happened in the brain. But if I ask you a complex maths problem, or a riddle, or even a programming issue, you're likely to think in your head.

For instance, I will ask you a maths question and try to think about what happens in your brain as you answer. 1258 * 2. Depending on your skill at mental calculus, you might think "8*2 is 16, 1250 * 2 is 2500, so it's 2516", or have some other more or less efficient way of thinking about it. That's reasoning, and it requires thinking one token at a time for you as well. A more complex problem might require you to first think about how to solve it before attempting it. GPT-4 is not different in that sense. It's just that you can literally see its thinking process as part of the response. Maybe GPT-5 will have a [thinking] part of an answer that will not be shown by default. But at this point it really just becomes a matter of cost / efficiency. Having GPT-4 think so hard about everything you ask is just very inefficient, the same way you won't have the same level of double-checking when estimating the cost of your meal at a restaurant or doing your taxes. 

## But it has blind spots

Another classic issue that we find is that GPT has bias, hallucinations etc. And that's a real problem. But I would not say it stops it from reasoning. All of us have bias, and some of us suffer from hallucinations or being confidently wrong. Would you say a flat-earther is devoid of the capacity of reasoning ? – fair enough, you might think that, I walked into that one – But personally, I think there is a world between a flat-earther, who is reasoning and reaches wrong conclusions, to say a cat or a rock. Being correct or being correct consistently is not a definition of reasoning, it's a definion of omniscience. 

## But does it have conscience

This is where I would draw the line. No, I don't think today GPT-4 has conscience. At this point it's very philosophical and down to my own beliefs, but I think consciousness appears over a long period of time, and requires a "self" to take care of. Whenever you start a conversation with an instance of GPT-4, you're essentially creating a whole new being, and killing it at the end of the conversation (or leaving it in stasis). The lack of long term memory, of an emotion centre (that reacts to external stimuli) are big limiters to anything like a consciousness emerging. But I'm also optimistic that those are problems that can be solved and that I am certain are worked on by very smart people at this very moment. GPT-4 is but a piece of that puzzle, but it is a significant one. GPT-4 is but a piece of that puzzle but it is a significant one. But until then I'll just keep working on projects with it, such as [ChartMyLife.ai](https://chartmylife.ai), a customisable life tracker that uses GPT-4 to turn mushy life events into data that you can chart and query.

