---
title: "DMR 2027"
edition: 2027
permalink: /2027/
---

__Welcome to DMR 2027, the Eighth International Workshop on Designing Meaning Representations!__

## Meaning Representations for Neuro-Symbolic Language Intelligence

<div class="notice" markdown="1">
**Status:** DMR 2027 has been proposed for the 2027 ACL conference cycle. The host conference, dates,
and submission deadlines will be announced here once the proposal is accepted. Please check back, or
watch the [ACL workshop announcements](https://www.aclweb.org/portal/) for updates.
</div>

## Workshop Topic and Motivation

Large language models (LLMs) and other foundation models have dramatically improved language generation,
information extraction, question answering, and many forms of linguistic analysis. Yet the semantic
structures underlying model outputs are rarely made explicit in a form that can be systematically inspected
or verified. This makes it difficult to determine which entities, events, relations, temporal structures,
modal commitments, discourse relations, or causal connections a model has actually inferred, and it
complicates verification, intervention, compositional reasoning, and explanation.

Decades of work in computational semantics have developed explicit meaning representations (MRs), including
Abstract Meaning Representation (AMR), Uniform Meaning Representation (UMR), Discourse Representation Theory
(DRT), Minimal Recursion Semantics (MRS), Prague tectogrammatical representations, UCCA, and related graph-
and logic-based formalisms. These representations make semantic structure inspectable and manipulable, and
many were designed to support inference. At the same time, symbolic representations have traditionally
required expensive annotation and specialized parsers, limiting their coverage and scalability.

DMR 2027 will focus on meaning representation as an *interface* between neural model learning and symbolic
reasoning. Rather than treating semantic parsing as an end in itself, the workshop asks how explicit
representations of meaning can provide structured supervision, intermediate reasoning states, editable
memories and world models, interfaces to theorem provers and planners, and constraints for reliable
generation. Conversely, it asks how LLMs can reduce the cost of constructing, extending, aligning, and using
symbolic MRs. This bidirectional perspective provides a concrete research program for neuro-symbolic NLP:
neural models supply broad coverage and learning capacity, while explicit semantic structures supply
compositionality, interpretability, controllability, and verifiable interfaces to reasoning.

The workshop brings together researchers in computational semantics, semantic parsing, foundation models,
knowledge representation, machine reasoning, multilingual NLP, information extraction, and agentic AI. Its
central scientific question is:

> How should meaning representations be designed, learned, and used so that they provide an effective
> interface between neural language models and symbolic reasoning systems?

## Topics of Interest

We invite long papers, short papers, position papers, resource papers, negative-results papers, and system
demonstrations on topics including:

- design, annotation, comparison, and formal properties of symbolic, distributed, and hybrid meaning representations;
- MRs for entities, events, semantic roles, coreference, temporal relations, modality, negation, causality, discourse structure, uncertainty, and attribution;
- LLMs that generate, revise, or reason over semantic graphs, logical forms, or other explicit structures;
- neural semantic parsing and generation, including few-shot, multilingual, low-resource, and human–AI collaborative annotation;
- MRs as structured memory, world models, plans, or intermediate states for language agents;
- integration of LLMs with theorem provers, constraint solvers, planners, knowledge bases, graph algorithms, and executable representations;
- semantic constraints for decoding, self-correction, factual verification, and controllable generation;
- neuro-symbolic approaches to natural-language inference, temporal and causal reasoning, question answering, information extraction, summarization, and tool use;
- multilingual, cross-lingual, multimodal, and culturally diverse meaning representation;
- evaluation of semantic equivalence, compositional generalization, logical consistency, faithfulness, robustness, and downstream reasoning utility.

## Format

DMR 2027 is planned as a one-day workshop combining invited talks, contributed oral presentations,
posters and demos, and a panel or structured discussion on the role of explicit semantic representations in
foundation models. Presenters will be asked to state both (i) the representational commitments of their work
and (ii) the capability — reasoning, verification, transfer, controllability, or interpretability — that the
representation enables.

All oral sessions will support remote presentation and questions through the host conference platform, and
poster authors unable to attend in person will be offered virtual presentation slots or an online poster
session, subject to the host conference's infrastructure.

## Important Dates

| Paper submission deadline      | To be announced |
|:------------------------------:|:---------------:|
| __Notification of acceptance__ | __To be announced__ |
| __Camera-ready papers due__    | __To be announced__ |
| __Workshop date__              | __To be announced__ |

Dates will be set in coordination with the host conference's workshop chairs.

## Invited Speakers and Shared Task

We plan to invite two speakers representing complementary perspectives — one from computational and formal
semantics, and one from neuro-symbolic or foundation-model reasoning. Speakers will be announced here once
confirmed.

Building on the [DMR 2026 shared task on UMR parsing]({{ '/2026/shared-task/' | relative_url }}), we are
considering a shared task that evaluates not only semantic parsing but also *representation-supported
reasoning*: systems would map text to a structured MR and answer controlled temporal, modal, causal, or
referential questions, or respond correctly after targeted interventions on the representation. A decision
will be announced along with the rest of the workshop schedule.

## Contact

<!-- TODO: replace with the DMR 2027 workshop mailing address once it has been created. -->
A workshop contact address will be announced with the call for papers. In the meantime, questions can be
directed to any of the [organizers]({{ '/2027/committees/' | relative_url }}).
