Machine Epistemology

Exploratory research into rule identification, generalisation, and conceptual abstraction in artificial agents.

Research Overview

Machine Epistemology is an ongoing independent research project investigating how artificial learning systems identify underlying rules from limited observations.

A central question is whether successful predictions demonstrate that a system has identified the correct underlying explanation, or whether alternative explanations remain consistent with the available evidence.

The project explores this distinction through controlled computational experiments, symbolic rule learning, and model evaluation.

Experiment 1 — Hidden Rule Identification

Objective

To investigate whether a learning algorithm can identify the correct underlying classification rule from a limited number of observations.

Methodology

A synthetic environment was constructed containing:

16 possible objects, represented by four binary attributes (A, B, C and D).

A hidden classification rule: A = 1 AND B = 1.

24 candidate rules consisting of conjunctions of two attribute conditions.

An initial training set of six randomly selected objects.

A seventh example deliberately selected to distinguish competing explanations.

The learner evaluated candidate rules against the observed training data.

Results

Measurement

Six examples

Seven examples

Rules consistent with training data

2

1

Correct predictions on shared held-out data

6/9

9/9

Held-out accuracy

66.67%

100%

Both learners were evaluated on the same nine objects that neither had seen during training.

Interpretation

The initial training observations were consistent with two different candidate rules. Both explained the observed data, but only one matched the hidden generating rule.

The deliberately selected seventh observation distinguished these competing explanations.

This illustrates why fitting the available observations is not necessarily equivalent to identifying the underlying rule.

Limitations

This experiment is a small, controlled demonstration rather than evidence of general autonomous conceptual discovery.

The hypothesis space was restricted to 24 predefined rules. The seventh example was deliberately selected rather than randomly sampled, and the six-example learner's selection depended on the rule-search ordering.

The experiment does not establish that similar improvements would occur across larger or more complex learning environments.

Repository Contents

Identify_Hidden_Rules_Machine_Epistemology.ipynb — Python experiment and explanations.

machine_epistemology_experiment_1.csv — Numerical results.

machine_epistemology_experiment_1.png — Visual comparison of prediction accuracy.

Reproducing the Experiment

Download the Jupyter notebook or open it in Google Colab.

Ensure the required Python libraries are available, including pandas and Matplotlib.

Execute the notebook cells in order.

Examine the candidate-rule comparisons, held-out predictions and generated results.

Future Research

Planned investigations include repeated trials across different training samples, additional model baselines, noisy observations, and tests of generalisation and transfer.

These experiments will investigate the conditions under which predictive success does or does not provide reliable evidence of underlying rule identification.

Research Status

Ongoing independent exploratory research.

The current repository documents an initial experiment and is intended to expand as further experiments are completed and evaluated.
