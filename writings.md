---
layout: default
title: Writings
permalink: /writings
---

# Writings

## How to solve your favorite research math problem with AI

It is common knowledge now that AI is extremely powerful, perhaps even super-human, at solving research-level math problems. ChatGPT, only in the last 2 years, has gone from barely being able to solve high school math problems to fully resolving and formalizing Millennium Prize problems. However, this might contrast with your own experience of trying and failing to solve research level math problems, even with the best models like GPT Astra or Claude Fable. Given below are some tips on how to get the best out of your subscription for solving your favorite problems. 

<details class="read-more" markdown="1">
<summary>Read the rest of this entry</summary>

### Almost nothing works

Every few days, we get a new harness/workflow to try out our problems with. These harnesses may do several things like decompose a problem into smaller sub-problems, instruct separate agents to attack different parts of the problem, keep a record of things tried, etc. However, it is likely that frontier models are doing all of these tasks under the hood anyway. Hence, adding these features on top may in fact hurt instead of help. This is exactly the result that our research group at Princeton has obtained as well, which we will be putting out in a few days. Any idea that you've thought of, if it works, chances are frontier labs have incorporated it into their model already (unless it is prohibitively expensive). We give some exceptions to this rule below, but having any of them work does depend somewhat somewhat on luck. 

### What does somewhat work is asking the same question several times in parallel, and keeping a record of failed attempts

When harnesses help, it is not because they've found a secret unlock to extract better reasoning from models that your plain prompt could not. More often than not, they are helpful because they are asking the model the same question several times, and choosing the best answer. They may state that they have obtained improved performance from a new technique, like having a prover and verifier working together for several rounds, but we were able to replicate the same accuracy in problem solving by just asking a model the same question several times and then choosing the best or most correct answer. Hence, simply asking your model the same question on 5 different tabs, and choosing the best output to seed the next round of attempts with, is a reliably good technique. 

Another thing that helps is having a centralized repository of failed attempts, why the attempts failed, etc. However, the returns on this may become apparent only over long horizon workflows. In other words, this becomes helpful if you keep working and iterating on the same problem over several hundred attempts. Of course it's more likely than not that if your model has been unable to solve your problem over several hundred attempts, you have to simplify it to a problem that it can solve. Re-wording your problem in different ways, like one may be able to sometimes re-word a problem from algebra as a problem in combinatorics, may be a really powerful technique. 

### It also helps if you attach relevant papers, whose techniques may be relevant

Something that reliably did help in increasing the number of problems that Gemini was able to solve was attaching papers that were relevant to the question that we were interested in. Note that the attached papers did not contain the answers to the questions, and were old enough that Gemini had almost certainly been trained on them. However, despite only attaching data that the model almost certainly knew about, the observed success rate increased markedly. If you're stuck on your problem, attaching 5-10 most relevant papers that you even vaguely suspect might help with a proof, could mean the difference between a proof and only partial or no progress.

If you can't think of relevant papers, pointing your model at particular fields or subfields that are unrelated to your stated problem might help. We've seen instances of mathematicians saying "explore fields that are orthogonal to this field, and might seem unrelated to the problem at hand", and seeing their model magically come up with a proof because it ended up reading a paper completely outside the mathematician's expertise.

### In each attempt, even if your model fails to answer the question, it must make falsifiable predictions

This is perhaps most important. More likely than not, your model will fail to solve the given problem in one attempt. In such circumstances, models end up ending their answers with "it might be fruitful to explore this route". This is not a falsifiable prediction, or at least will take lots of time and effort to falsify. What might work best is if the models, to the best of their understanding, make a precise and falsifiable conjecture/lemma, which if true will complete the proof. This seeds your next attempt with a promising idea that may be true (perhaps after sufficient repair), or rule out a certain direction for future attempts. 

This was repeatedly the pattern that was observed in the [reasoning walkthrough](https://cdn.openai.com/pdf/reasoning-walkthroughs.pdf) put out by OpenAI earlier this year, explaining how their models were able to solve 10 big problems in Mathematics. Forcing your models to be precise in their predictions, especially if they are thoroughly reasoned and tested, can be very powerful. 

These are some of the observations that I've had while trying to solve research math questions with frontier models. I'll be grateful for feedback and/or corrections. Thanks! 

</details>


## How to start out with AI tools for math research

### Access to frontier models

The first thing that one may do is get a subscription to a good LLM. The strongest models that come to mind are ChatGPT, Claude and Gemini. All three have $20/month subscriptions as well as $200/month subscriptions. If you are mainly buying subscriptions for understanding mathematical documents, the $20 subscription is sufficient. However, if you want access to better reasoning models or are doing a lot of coding with AI agents, you may want to invest in the $200/month subscription. Note that OpenAI also offers access to its best models to academics free of cost. You may find more information about it [here](https://openai.com/index/chatgpt-for-academic-researchers/). 

<details class="read-more" markdown="1">
<summary>Read the rest of this entry</summary>

### Access to open source models

Alternatively, in case you are worried about data privacy or don't want to support big frontier AI companies, you may use open source models. Some models are small enough to run on your laptop, although they offer limited reasoning capabilities. A good resource for downloading open source models is [Huggingface](https://huggingface.co/).

In case you want access to better reasoning models that you're unable to run on your laptop, but also care about data privacy, you may want to enroll in [Open Math Model](https://www.openmathmodel.org/) hosted at SAIR. They may be compute constrained at the moment, but are in the process of expanding access. Another option is that you may buy API credits, and then use them as you go. A useful website for buying credits for open source models (as well as closed source models) is [OpenRouter](https://openrouter.ai/). Note that companies like DeepSeek explicitly state that they offer subsidized access to their models because they will train on your data. Hence, you may want to read the fine print before using both closed source and open source models. 

### Having different models work together

Note that although ChatGPT, Claude and Gemini all offer extremely strong reasoning capabilities, the biggest wins come from combining their capabilities. One way to do that is to make them work together, by making them read and critique each others' answers for several rounds. You may do so through [Claude Tuner](https://claudetuner.com/multiai/). If you have subscriptions to any subset of these three models, you may log into your accounts, and then go to "Debate" mode on Claude Tuner. Now if you ask a question in this mode, you'll have a moderator (say ChatGPT) moderating a debate between two or more models for up to 50 rounds (you can raise this limit). You can of course do this through a personalized harness as well, although Claude Tuner is much easier to use. Note that you only need subscriptions, and not API access, to use it. 

All in all, the best way to start with LLMs for math research is to get access to a good model, and start plugging away. Hope that this article has been useful!

</details>


