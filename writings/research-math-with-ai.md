---
layout: default
title: How to solve your favorite research math problem with AI
permalink: /writings/research-math-with-ai/
---

<p><a href="{{ '/writings/' | relative_url }}">Back to writings</a></p>

# How to solve your favorite research math problem with AI

It is common knowledge now that AI is extremely powerful, perhaps even super-human, at solving research-level math problems. ChatGPT, only in the last 2 years, has gone from barely being able to solve high school math problems to fully resolving and formalizing Millennium Prize problems. However, this might contrast with your own experience of trying and failing to solve research level math problems, even with the best models like GPT Astra or Claude Fable. Given below are some tips on how to get the best out of your subscription for solving your favorite problems.

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
