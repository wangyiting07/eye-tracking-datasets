# Eye Tracking Datasets

A curated collection of eye tracking datasets that may be useful for future research projects.

The catalog prioritizes datasets with **raw gaze time series**, high sampling rates, useful eye movement annotations such as fixations, saccades, microsaccades, and smooth pursuit, and datasets where the **task stimuli are available**. Stimulus availability is particularly important for future models that jointly learn from gaze and the visual or textual content being viewed. Strong multimodal datasets containing eye tracking are also included.

## Dataset index

| Dataset | Released | Sampling rate | Raw gaze | Event labels | Task stimuli available | Modalities | Notes |
|---|---|---:|---|---|---|---|---|
| [Active Visual Semantics](datasets/active-visual-semantics.md) | 2026-09-01 | 1000 Hz | Yes | Fixation, saccade | **Yes** — 4,080 natural scene images | Eye tracking, MEG, MRI, behavioural data | Natural scene free viewing; 4,080 scenes; 200,000+ fixation epochs |

## What gets recorded

For each approved dataset, the detailed entry should capture:

- publication or release date
- eye tracker and sampling rate
- whether raw gaze trajectories are available
- available event labels
- participants and task
- **whether the task stimuli are available, what modality they are, and how they can be accessed**
- other modalities, when applicable
- access links and citation
- why the dataset may be useful
- important limitations or caveats

## Status labels

- **Approved**: potentially useful and worth retaining in this catalog
- **Multimodal**: eye tracking is accompanied by another major modality such as EEG, MEG, MRI, video, or physiological signals

This repository is intended as a lightweight research reference rather than an exhaustive database of eye tracking datasets.
