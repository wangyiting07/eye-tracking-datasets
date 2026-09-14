# Eye Tracking Datasets

A curated collection of eye tracking datasets that may be useful for future research projects.

The catalog prioritizes datasets with **raw gaze time series**, high sampling rates, useful eye movement annotations such as fixations, saccades, microsaccades, and smooth pursuit, and datasets where the **task stimuli are available**. Stimulus availability is particularly important for future models that jointly learn from gaze and the visual or textual content being viewed. Strong multimodal datasets containing eye tracking are also included.

## Dataset index

| Dataset | Released | Sampling rate | Raw gaze | Event labels | Task stimuli available | Modalities | Reference | Notes |
|---|---|---:|---|---|---|---|---|---|
| [Active Visual Semantics](datasets/active-visual-semantics.md) | 2026-09-01 | 1000 Hz | Yes | Fixation, saccade | **Yes** — 4,080 natural scene images | Eye tracking, MEG, MRI, behavioural data | Sulewski et al., 2026 | Natural scene free viewing; 4,080 scenes; 200,000+ fixation epochs |

## What gets recorded

For each approved dataset, the detailed entry should capture:

- publication or release date
- eye tracker and sampling rate
- whether raw gaze trajectories are available
- available event labels
- participants and task
- **whether the task stimuli are available, what modality they are, and how they can be accessed**
- other modalities, when applicable
- **the official dataset or primary paper citation**
- **dataset licence and attribution requirements**
- **stimulus provenance and stimulus licence information when applicable**
- access links
- why the dataset may be useful
- important limitations or caveats

## Attribution and licensing

This repository is a research catalog. It contains summaries, citations, and links to third-party datasets rather than redistributing the datasets themselves.

Copyright and licensing remain with the original dataset creators and upstream content owners. Anyone using a listed dataset should consult the official dataset documentation and comply with its current licence, citation requirements, ethical-use terms, and any separate licences applying to task stimuli.

For datasets whose stimuli originate from another resource, such as image, text, video, or audio collections, the upstream stimulus licence may differ from the licence of the eye tracking dataset itself. The relevant stimulus provenance and licence information should therefore be checked before reproducing or redistributing those materials.

## Status labels

- **Approved**: potentially useful and worth retaining in this catalog
- **Multimodal**: eye tracking is accompanied by another major modality such as EEG, MEG, MRI, video, or physiological signals

This repository is intended as a lightweight research reference rather than an exhaustive database of eye tracking datasets.
