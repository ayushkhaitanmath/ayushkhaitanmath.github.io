---
layout: default
title: Research
permalink: /research
---

<section id="research" class="res">

  <h1 class="res__title">Research</h1>

  <!-- ===== AI for Mathematics ===== -->
  <article class="card">
    <h2 class="card__title">AI for Mathematics</h2>
    <div class="card__body">
      <p>My work in this area involves constructing AI tools that can be useful in mathematics research. This involves training and fine-tuning LLMs, and integrating LLMs with computer algebra systems. Using an <a href="https://arxiv.org/abs/2510.12350">LLM+CAS framework</a>, we were recently able to answer a question of Terence Tao by constructing an AI tool that can prove research-level inequalities from several mathematical domains.</p>
      <p>I also run a large research group of undergraduates, in which we construct AI tools that can be useful for Mathematicians. One group of students has built <a href="https://github.com/SiddarthNarayanan01/darwin">Darwin</a> a version of Google’s FunSearch that's faster and more efficient for some types of computations, especially combinatorics. Using this, they were able to construct a combinatorial example in 25 minutes that had previously taken 3 days of compute. Another group of students has <a href="https://ricci-website.vercel.app">fine-tuned</a> an LLM on Mathematica’s Ricci package.</p>
      <p>I also co-organize an <a href="https://ai-math-seminar.github.io/seminar/">AI for Mathematics</a> seminar. I started the AI and Mathematics <a href="/seminar.html">seminar</a> at Rutgers in Spring 2025. This semester, I am teaching an Intro to Proofs course based on Lean, and a graduate course in machine learning.</p>
    </div>
  </article>

  <!-- ===== Geometric analysis & conformal geometry ===== -->
  <article class="card">
    <h2 class="card__title">Geometric analysis and conformal geometry</h2>
    <div class="card__body">
      <p>In my PhD, I have <a href="https://arxiv.org/abs/2308.02061">constructed</a> an infinite family of fully non-linear analogues of Perelman’s W-functional, that are monotone along the Ricci flow.</p>
      <p>During my postdoc, I have fully proved a conjecture of Bhargav Narayanan, and partially <a href="https://arxiv.org/abs/2505.12178">solved</a> the problem of proving sharp lower bounds on the permanent of a matrix, using tools from geometric analysis. Proving sharp lower bounds on the permanent of a matrix is an old, central problem in statistical mechanics, theoretical computer science and combinatorics, and we were surprisingly able to make progress on this question using monotone flows and differential operators.</p>
    </div>
  </article>

</section>

<style>
  :root{
    --bg: var(--site-background);
    --ink: var(--site-ink);
    --mute: var(--site-muted);
    --soft: var(--site-muted);
    --line: var(--site-line);
    --chip: var(--site-surface);
    --r: 14px;
  }

  .res{ background: var(--bg); max-width: 900px; }
  .res__title{ margin: 0 0 6px 0; font-size: 2rem; line-height: 1.2; color: var(--ink); }

  .card{ padding: 16px 0 18px 0; border-top: 1px solid var(--line); }
  .card:first-of-type{ border-top: 0; }

  .card__title{ margin: 0 0 8px 0; font-size: 1.35rem; font-weight: 650; color: var(--ink); }

  .card__body{
    background: var(--chip);
    border: 1px solid var(--line);
    border-radius: var(--r);
    padding: 14px 16px;
    color: var(--soft);
    font-size: 0.98rem;
    line-height: 1.55;
  }

  .card__body a{
    color: var(--site-link);
    text-decoration: none;
    border-bottom: 1px dotted var(--site-link-underline);
  }
  .card__body a:hover{ border-bottom-color: transparent; }

  @media (max-width: 640px){
    .card__title{ font-size: 1.2rem; }
    .card__body{ font-size: 0.96rem; }
  }
</style>
