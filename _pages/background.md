---
permalink: /Background/
title: "Background"
classes: wide
sidebar:
- title: "Terminology"
- text: "<p><b>Human-in-the-Loop Bayesian Optimization (HITL BO)</b>, An approach that updates a probabilistic model with user feedback to propose the next design to test.</p>
<p><b>Bayesian Optimization (BO)</b>, Sample-efficient search for the optimum of a black-box function using a surrogate model and an acquisition function.</p>
<p><b>Multi-Objective BO (MOBO)</b>, BO that targets multiple objectives at once, outcomes are summarized with Pareto fronts and hypervolume.</p>
<p><b>Surrogate model</b>, A probabilistic model, often a Gaussian process, that predicts outcomes across the design space with uncertainty.</p>
<p><b>Acquisition function</b>, A rule that balances exploration and exploitation to select the next query, for example Expected Improvement.</p>"
---

In many HCI problems, designers face large parameter spaces, limited budgets, and objectives that conflict. Usability, workload, trust, accessibility, and performance pull in different directions, the mapping from parameters to outcomes is unknown and noisy. Standard iteration is slow and risks missing good configurations.

HITL BO provides a principled alternative. A surrogate model estimates outcomes from observed data, an acquisition function proposes the next configuration, users supply quick judgments or task results, the loop repeats with far fewer trials than grid search or ad hoc tuning. With MOBO, designers balance multiple goals and read out trade-offs via the Pareto front rather than a single score.

Evidence from vision, haptics, text entry, and automotive interfaces shows that HITL BO can tune layouts, timings, intensities, and styles with fewer samples, while keeping humans in control of what “good” means. The method is suitable for personalization, group-aware tuning, and adaptive systems that must work across abilities.

Methodological challenges remain. User feedback is noisy, high-dimensional spaces slow learning, multi-objective settings require careful analysis, repeated queries can fatigue participants, fairness can drift toward majority preferences. Practical workflows address these risks with warm starts, dimensionality reduction, adaptive stopping, and reporting that includes Pareto sets and hypervolume.

This workshop introduces HITL BO as a practical method for HCI. Participants learn core concepts, see a live Python to Unity loop, map their own problems to HITL BO pipelines, and discuss limits and ethics. Materials include notebooks, a Unity sample, checklists, and a curated bibliography, enabling attendees to apply the method in their projects.
