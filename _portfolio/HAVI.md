---
title: "Mapping Legal Logic: Argumentation Graphs for AI"
excerpt: "This grant proposal outlines a neuro-symbolic pipeline utilizing Quantitative Bipolar Argumentation Frameworks (QBAFs) to resolve complex, contradictory legal texts. By decoupling LLM semantic parsing from deterministic dialectical logic, the project aims to limit AI hallucinations and computationally model defeasible legal reasoning at scale."
collection: portfolio
permalink: /portfolio/HAVI
---

## Overview

This grant proposal, developed in collaboration with researchers from the Polish Academy of Sciences, Jagiellonian University, and the LegalTech startup RegAlly, addresses the structural brittleness of linear LLM "Chain-of-Thought" reasoning when confronted with contradictory legal texts. The project outlines a hybrid neuro-symbolic pipeline that abandons stochastic text generation in favor of Graph-Based Reasoning, specifically utilizing Quantitative Bipolar Argumentation Frameworks (QBAFs) layered over a live regulatory database. By restricting the LLM to semantic parsing and handing the actual dialectical logic to a deterministic algorithm (DF-QuAD), the proposal aims to solve the pervasive issue of "legal hallucinations" while transforming abstract jurisprudential theories of defeasibility into computationally testable, empirical science at scale

## Project Description

# Project Abstract

Current Large Language Models (LLMs) fail at complex legal reasoning because they rely on
linear "Chain-of-Thought" generation, which collapses into hallucinations when faced with
contradictory laws. Law is inherently non-monotonic and "defeasible"—specific exceptions
routinely override general rules. Partnering with a commercial European regulatory
intelligence platform, we propose a neuro-symbolic upgrade: replacing linear LLM reasoning
with Quantitative Bipolar Argumentation Frameworks (QBAFs). We will map thousands of
interacting legal norms into a mathematical graph of attacking and supporting nodes. By
using the DF-QuAD algorithm to calculate the "dialectical strength" of conflicting rules, we
remedy the AI's inability to weigh contradictory evidence. Simultaneously, we provide
humanities scholars with an innovative computational tool to empirically map normative
conflicts and test theories of legal argumentation on real-world datasets.

# Humanities Research Question:

How can the philosophical concept of “defeasibility”—the vulnerability of legal conclusions to
limitations, counterarguments, and competing normative reasons—be computationally
modeled and empirically tested on large-scale regulatory datasets? Rather than treating
legal conflict as abstract collisions, we examine how overlapping regulatory regimes interact
in practice. Using a live European database, we will formalize tensions between distinct
legally protected values (e.g., AI transparency vs. trade secret protection, or data privacy vs.
bias mitigation obligations). By mapping how norms across domains create exceptions and
interpretive reasons, we will capture the structural topology of legal argumentation. This
advances legal philosophy from an abstract framework into a data-driven empirical science,
allowing scholars to computationally measure real-world legal harmonization.

# AI Research Question:

How can we overcome the brittleness and hallucinations of linear LLM "Chain-of-Thought"
prompting in contradictory datasets? Generative models struggle with non-monotonic logic.
This project layers a Quantitative Bipolar Argumentation Framework (QBAF) over a
regulatory retrieval system to create a graph-based reasoning pipeline. Can we use LLMs
strictly as semantic parsers to extract "attacking" and "supporting" rules, delegating conflict
resolution to a deterministic algorithm (DF-QuAD)? Anticipating the critique that this
"muzzles" the LLM, we argue this is a vital neuro-symbolic upgrade. By dividing labor into a System 1 (semantic perception) and System 2 (logical reasoning) architecture, the graph
acts as a mathematical guardrail. We aim to replace stochastic generation with explainable
"dialectical strength" calculations, advancing AI's capacity for defeasible reasoning while
eliminating hallucinations.

---