# Active Visual Semantics

**Status:** Approved  
**Type:** Multimodal eye tracking dataset  
**Release date:** 2026-09-01

## Summary

Active Visual Semantics, or AVS, combines high frequency eye tracking with MEG during free viewing of natural scenes. It is potentially useful for representation learning, multimodal modelling, fixation level analysis, and studies linking gaze behaviour to visual semantics and neural activity.

## Eye tracking details

- **Sampling rate:** 1000 Hz
- **Raw gaze trajectories:** Yes
- **Eye movement events:** Fixations and saccades are explicitly available
- **Microsaccade labels:** Not explicitly documented as a dedicated label set
- **Smooth pursuit labels:** Not reported
- **Pupil data:** Available

## Task and scale

Participants freely viewed natural scenes while eye movements and MEG were recorded. The dataset contains 4,080 natural scenes and more than 200,000 fixation epochs. Fixations can be linked to visual semantic information, including object category labels.

## Modalities

- Eye tracking
- MEG
- Structural MRI
- Behavioural annotations
- Scene and object semantics

## Why it may be useful

AVS is especially interesting because it combines:

- raw gaze sampled at 1000 Hz
- fixation and saccade annotations
- naturalistic free viewing
- synchronized neurophysiology
- semantic labels at the fixation level

This makes it useful for future work on multimodal gaze modelling, eye movement representation learning, gaze conditioned visual models, and analyses of the relationship between eye movements and neural responses.

## Caveats

The dataset should not currently be treated as a dedicated microsaccade benchmark. Saccades are annotated, but a separate microsaccade label set was not clearly documented in the release information reviewed when this entry was created.

## Resources

- Dataset documentation: https://avsdataset.com/
- Public data access and project resources should be checked from the official AVS documentation for the latest locations and version information.

## Catalog note

Added to this repository as a potentially useful future research dataset because it provides raw high frequency gaze data together with event annotations and rich multimodal context.
