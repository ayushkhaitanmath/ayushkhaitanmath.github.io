---
layout: default
title: Publications
permalink: /publications
---

<!-- Publications with always-visible summaries -->
<section id="publications" class="pubs">

  <h1 class="pubs__title">Publications</h1>

  <!-- Paper: mini-Lean-agent -->
  <article class="pub">
    <h2 class="pub__title"><em>Do Theorem Provers Need Theorem-Proving Agents? mini-Lean-agent: A Coding-Agent Baseline for Lean</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Tomas Ortega, Simon Park, Ayush Khaitan, Liam Fowl, <a href="https://sites.math.rutgers.edu/~alexk/">Alex Kontorovich</a>, <a href="https://www.cs.princeton.edu/~arora/">Sanjeev Arora</a></div>
    <div class="pub__meta">6th Workshop on Mathematical Reasoning and AI (MATH-AI), NeurIPS 2026 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2610.17331">arXiv:2610.17331</a></div>
    <div class="pub__summary">
      We introduce mini-Lean-agent, a deliberately minimal agent for Lean whose only model-visible tool is bash, with a separate trusted evaluator checking the final output. On the Putnam 2025 benchmark it solves 7/12 problems with Gemini 3.8 Flash (versus 4/12 for AxProverBase), and all 12/12 with Astra at an average cost of $1.28 per problem. This suggests that a generic coding agent should be the standard baseline for evaluating theorem-proving infrastructure.
    </div>
  </article>

  <!-- Paper: Semantic equivalence in formalization -->
  <article class="pub">
    <h2 class="pub__title"><em>Improving semantic equivalence in research-level math formalization</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan, Liam Fowl, Tomas Ortega, <a href="https://sites.math.rutgers.edu/~alexk/">Alex Kontorovich</a>, <a href="https://www.cs.princeton.edu/~arora/">Sanjeev Arora</a></div>
    <div class="pub__meta">6th Workshop on Mathematical Reasoning and AI (MATH-AI), NeurIPS 2026 &nbsp;•&nbsp; <a href="https://openreview.net/forum?id=OFimGMpfHW">OpenReview</a></div>
    <div class="pub__summary">
      A Lean formalization is never a word-for-word translation of a paper: it changes definitions, strengthens hypotheses and adds lemmas the paper never mentions. We collect 4,076 audited examples of such departures from Lean projects formalizing research-level mathematics, and show that training on them nearly doubles complete proofs (11% to 20%) and raises the share of faithful statements from 30% to 39%.
    </div>
  </article>

  <!-- Paper: 100-conjecture calibration study -->
  <article class="pub">
    <h2 class="pub__title"><em>Does a Frontier Large Language Model Know What It Can Solve? A 100-Conjecture Calibration Study</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan, Liam Fowl, Tomas Ortega, <a href="https://sites.math.rutgers.edu/~alexk/">Alex Kontorovich</a>, <a href="https://www.cs.princeton.edu/~arora/">Sanjeev Arora</a></div>
    <div class="pub__meta">6th Workshop on Mathematical Reasoning and AI (MATH-AI), NeurIPS 2026 &nbsp;•&nbsp; <a href="https://openreview.net/forum?id=CT9WOChlRl">OpenReview</a></div>
    <div class="pub__summary">
      We test how a frontier LLM's stated confidence tracks its actual success on 87 audited open conjectures in geometric analysis. The model was strongly overconfident (mean stated probability 0.617 versus an observed success rate of 0.103), yet its probabilities still ranked problems in the right direction (AUROC 0.714). All proofs were formalized in Lean and checked for semantic equivalence with their informal statements.
    </div>
  </article>

  <!-- Paper: Geometrization conjecture formalization -->
  <article class="pub">
    <h2 class="pub__title"><em>A Lean Formalization of the Hamilton–Perelman Proof of Thurston's Geometrization Conjecture</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Yuan Liao, <a href="https://qinziyang.com/">Ziyang Qin</a>, Jui-Hui Chung, Ayush Khaitan, Zhengyang Zhang, Hongzhou Lin, Zijian Zhang, Ligeng Zhu, Peng Lu, <a href="https://mathweb.ucsd.edu/~bechow/">Bennett Chow</a></div>
    <div class="pub__meta">Preprint, 2026 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2610.13897">arXiv:2610.13897</a></div>
    <div class="pub__summary">
      We formalize in Lean the Hamilton–Perelman Ricci-flow proof of Thurston's geometrization conjecture. The paper reproduces the public Lean statement of the theorem, explains its geometric interpretation, and records how the formalization was verified.
    </div>
  </article>

  <!-- Paper: Poincaré conjecture formalization -->
  <article class="pub">
    <h2 class="pub__title"><em>A Lean Formalization of the Hamilton–Perelman Proof of the Three-Dimensional Poincaré Conjecture</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> <a href="https://qinziyang.com/">Ziyang Qin</a>, Yuan Liao, Ayush Khaitan, <a href="https://mathweb.ucsd.edu/~bechow/">Bennett Chow</a></div>
    <div class="pub__meta">Preprint, 2026 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2609.33842v1">arXiv:2609.33842</a></div>
    <div class="pub__summary">
      We formalize the smooth three-dimensional Poincaré conjecture, together with the Moise smoothing theorem, yielding the topological three-dimensional Poincaré conjecture. The smooth proof follows the Hamilton--Perelman route through Ricci flow with surgery and finite-time extinction.
    </div>
  </article>

  <article class="pub">
    <h2 class="pub__title"><em>O-Forge: An LLM + Computer Algebra Framework for Asymptotic Analysis</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan, <a href="https://www.cc.gatech.edu/people/vijay-ganesh">Vijay Ganesh</a></div>
    <div class="pub__meta">Submitted, 2025 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2510.12350">arXiv:2510.12350</a></div>
    <div class="pub__summary">
      We build an LLM+CAS framework that proves research‑level asymptotic inequalities. Using it, we resolve multiple questions from MathOverflow and other research forums. This answers a <a href="https://mathoverflow.net/a/463940/91878">question</a> <a href="https://terrytao.wordpress.com/2025/05/01/a-proof-of-concept-tool-to-verify-estimates/">posed</a> <a href="https://terrytao.wordpress.com/2025/05/09/a-tool-to-verify-estimates-ii-a-flexible-proof-assistant/comment-page-1/#comment-688872">by</a> Terence Tao. We are grateful for Terence's support for our project, including his highlighting of our tool <a href = "https://mathstodon.xyz/@tao/115379172603958618">here</a>. 
    </div>
  </article>

  <article class="pub">
    <h2 class="pub__title"><em>Local and global conformal invariants of submanifolds</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> <a href="https://sites.google.com/view/jeffreyscase">Jeffrey Case</a>, Ayush Khaitan, <a href="https://sites.google.com/view/yuehjulin">Yueh‑Ju Lin</a>, <a href="https://aaron-tyrrell.com">Aaron Tyrrell</a>, <a href="https://www.genealogy.math.ndsu.nodak.edu/id.php?id=241215">Wei Yuan</a></div>
    <div class="pub__meta">Submitted &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2604.08372">arXiv:2604.08372</a></div>
    <div class="pub__summary">We develop methods for constructing and computing conformal invariants of submanifolds, with a particular emphasis on conformal submanifold scalars and conformally invariant integrals of natural submanifold scalars.</div>
    </article>

  <!-- Paper: Elementary symmetric polynomials -->
  <article class="pub">
    <h2 class="pub__title"><em>Elementary symmetric polynomials under the fixed point measure</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan, <a href="https://sites.math.rutgers.edu/~narayanan/">Bhargav Narayanan</a>, <a href="https://sites.google.com/site/ishanmata">Ishan Mata</a></div>
    <div class="pub__meta">Submitted, 2025 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2505.12178">arXiv:2505.12178</a></div>
    <div class="pub__summary">
      We prove a surprising inhomogeneous inequality for symmetric polynomials, fully confirming a conjecture of Bhargav Narayanan. The result advances the program of obtaining sharp unconditional lower bounds on the permanent of a matrix.
    </div>
  </article>

  <!-- Paper: Poincaré–Einstein -->
  <article class="pub">
    <h2 class="pub__title"><em>Computing renormalized curvature integrals on Poincaré–Einstein manifolds</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> <a href="https://sites.google.com/view/jeffreyscase">Jeffrey Case</a>, Ayush Khaitan, <a href="https://sites.google.com/view/yuehjulin">Yueh‑Ju Lin</a>, <a href="https://aaron-tyrrell.com">Aaron Tyrrell</a>, <a href="https://www.genealogy.math.ndsu.nodak.edu/id.php?id=241215">Wei Yuan</a></div>
    <div class="pub__meta"><em>Advances in Mathematics</em> <strong>496</strong> (2026), 110991 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2404.11319">arXiv:2404.11319</a> <a href="https://doi.org/10.1016/j.aim.2026.110991">Journal link</a></div>
    <div class="pub__summary">
      We describe a general procedure for constructing renormalized curvature integrals on Poincaré–Einstein manifolds.
    </div>
  </article>

  <!-- Paper: Ambient metric with density + Ricci flow -->
  <article class="pub">
    <h2 class="pub__title"><em>Ambient metric for manifolds with density and the Ricci flow</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan</div>
    <div class="pub__meta"><em>Advances in Mathematics</em> <strong>488</strong> (2026), 110787 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2308.02061">arXiv:2308.02061</a> <a href="https://www.sciencedirect.com/science/article/pii/S0001870826000095">Journal link</a></div>
    <div class="pub__summary">
      We construct fully non‑linear analogues of Perelman’s W‑functional that are monotone along the Ricci flow, and stationary only for shrinking Ricci solitons. We do so by constructing a Fefferman–Graham ambient metric for manifolds with density.
    </div>
  </article>

  <!-- Paper: Weighted ambient metric -->
  <article class="pub">
    <h2 class="pub__title"><em>The weighted ambient metric</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> <a href="http://www.personal.psu.edu/jqc5026/">Jeffrey S. Case</a>, Ayush Khaitan</div>
    <div class="pub__meta"><em>SIGMA</em> <strong>18</strong> (2022), 086, 21 pages &nbsp;•&nbsp; <a href="https://www.emis.de/journals/SIGMA/2022/086/">Journal link</a></div>
    <div class="pub__summary">
      We construct the Fefferman–Graham ambient metric for smooth metric measure spaces.
    </div>
  </article>

  <!-- Paper: GJMS (weighted) -->
  <article class="pub">
    <h2 class="pub__title"><em>GJMS operators of smooth metric measure spaces</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan</div>
    <div class="pub__meta"><em>The Journal of Geometric Analysis</em> <strong>36</strong> (2026), no. 6, 210 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2203.04719">arXiv:2203.04719</a> <a href="https://link.springer.com/epdf/10.1007/s12220-026-02466-1?sharing_token=ozusi97-JFONwxa-nMNQD_e4RwlQNchNByi7wbcMAY43JlAUhr1u8GrIZ9U_EJ8i8bMOAFvRXhec1z4izu0_xlmOPCK8GWo6iV45qzTRhzaj8exrl7AXK2jfpe0x4Iojk7jwcnAYWLujrnuOr6BMSJaOJNxVwJx4f67qX1RCYEc%3D">Journal link</a></div>
    <div class="pub__summary">
      We construct GJMS operators for smooth metric measure spaces, and prove several properties.
    </div>
  </article>

  <!-- Paper: Weighted renormalized volume coefficients -->
  <article class="pub">
    <h2 class="pub__title"><em>Weighted renormalized volume coefficients</em></h2>
    <div class="pub__authors"><strong>Authors:</strong> Ayush Khaitan</div>
    <div class="pub__meta"><em>Differential Geometry and its Applications</em> <strong>105</strong> (2026), 102431 &nbsp;•&nbsp; <a href="https://arxiv.org/abs/2205.06018">arXiv:2205.06018</a> <a href="https://doi.org/10.1016/j.difgeo.2026.102431">Journal link</a></div>
    <div class="pub__summary">
      We construct renormalized volume coefficients for smooth metric measure spaces and prove several key properties.
    </div>
  </article>

</section>

<!-- Page-local styles using the shared site palette -->
<style>
  /* Palette + spacing */
  :root{
    --bg: var(--site-background);           /* page background */
    --surface: var(--site-background);      /* article surface */
    --t-ink: var(--site-ink);        /* title/body text */
    --t-mute: var(--site-muted);       /* secondary text */
    --t-soft: var(--site-muted);       /* summary text */
    --line: var(--site-line);         /* light rule/border */
    --chip: var(--site-surface);         /* off-white for the summary box */
    --link: var(--site-link);         /* muted teal */
    --link-underline: var(--site-link-underline);
    --r: 14px;               /* rounded radii */
    --x: 18px;               /* horizontal rhythm */
    --y: 14px;               /* vertical rhythm */
  }

  /* Scope styles to this page so we don't fight your site theme */
  .pubs{ 
    background: var(--bg);
    max-width: 900px;
  }
  .pubs__title{
    margin: 0 0 4px 0;
    font-size: 2rem;
    line-height: 1.2;
    color: var(--t-ink);
  }
  .pubs__intro{
    margin: 0 0 20px 0;
    color: var(--t-mute);
    font-size: 1rem;
  }

  .pub{
    padding: calc(var(--y) * 1.2) 0;
    border-top: 1px solid var(--line);
  }
  .pub:first-of-type{ border-top: 0; }

  .pub__title{
    margin: 0 0 6px 0;
    font-size: 1.35rem;
    font-weight: 650;
    color: var(--t-ink);
  }
  .pub__title em{ font-style: italic; }

  .pub__authors,
  .pub__meta{
    margin: 2px 0;
    font-size: 0.98rem;
    color: var(--t-mute);
  }

  .pub__meta a, .pub__authors a{
    color: var(--link);
    text-decoration: none;
    border-bottom: 1px dotted var(--link-underline);
  }
  .pub__meta a:hover, .pub__authors a:hover{
    border-bottom-color: transparent;
  }

  /* Summary box: small, crisp, relaxed */
  .pub__summary{
    margin-top: 10px;
    padding: 12px 14px;
    background: var(--chip);
    border: 1px solid var(--line);
    border-radius: var(--r);
    color: var(--t-soft);
    font-size: 0.95rem;
    line-height: 1.5;
  }

  /* Nice rhythm on narrow screens */
  @media (max-width: 640px){
    .pubs{ padding-right: 2px; }
    .pub__title{ font-size: 1.2rem; }
    .pub__summary{ font-size: 0.94rem; }
  }
</style>
