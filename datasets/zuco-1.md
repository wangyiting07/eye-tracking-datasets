# ZuCo 1.0

**Status:** Approved  
**Type:** Multimodal eye tracking and EEG dataset  
**Original publication:** 2018  
**NEMAR BIDS release:** 2026-09-16  
**Latest noted NEMAR update:** 2026-10-09

## Summary

ZuCo 1.0 combines high-resolution eye tracking with 128-channel EEG during natural sentence reading. The 2026 NEMAR release makes the dataset easier to reuse through a standardized BIDS-style archive with continuous gaze recordings and event metadata.

## Eye tracking details

- **Eye tracker:** EyeLink 1000
- **Sampling rate:** 500 Hz
- **Raw gaze trajectories:** Yes
- **Event annotations:** Fixations, saccades, and blinks
- **Microsaccade labels:** Not reported as a dedicated annotation set
- **Smooth pursuit labels:** Not applicable to the reading paradigm
- **Pupil information:** Included in the continuous eye tracking recordings

## Participants and task

- **Participants:** 12
- **Task:** Natural sentence reading
- Eye tracking and EEG were recorded synchronously during reading.

## Task stimuli

- **Task stimuli available:** **Yes**
- **Stimulus modality:** Text / sentences
- **Stimulus access:** Sentence materials are represented in the dataset/task files and associated metadata
- **Why this matters:** Text content can be aligned with gaze trajectories and EEG, making the dataset useful for stimulus-guided language-and-gaze representation learning

## Modalities

- Eye tracking
- 128-channel EEG

## Why it may be useful

ZuCo 1.0 is particularly relevant for:

- gaze-conditioned language modeling
- joint text, gaze, and EEG representation learning
- fixation and saccade modeling during reading
- multimodal foundation models for cognitive and linguistic signals
- stimulus-guided sequence modeling where the viewed text is explicitly known

The 500 Hz sampling rate is also substantially higher than many multimodal public datasets.

## 2026 update

The noteworthy 2026 change is the NEMAR-hosted BIDS-formatted release, which standardizes the archive structure and metadata and exposes continuous eye tracking together with event annotations in a more reusable form.

A subsequent NEMAR version update was posted on 2026-10-09. This catalog records that version change but does not claim a specific content change unless documented by the archive maintainers.

## Citation

Hollenstein, N., Rotsztejn, J., Troendle, M., Pedroni, A., Zhang, C., & Langer, N. (2018). ZuCo, a simultaneous EEG and eye-tracking resource for natural sentence reading. *Scientific Data, 5*, 180291. https://doi.org/10.1038/sdata.2018.291

## Licence and attribution

Use of the dataset should follow the licence and citation terms listed by the official ZuCo / NEMAR distribution.

This repository does not redistribute the recordings or sentence materials. Users should verify the current archive licence and any upstream text-source restrictions before redistribution.

## Resources

- NEMAR dataset: https://www.nemar.org/dataset/nm000278
- Original paper: https://doi.org/10.1038/sdata.2018.291

## Catalog note

Added as an approved dataset because it provides public 500 Hz raw gaze, fixation/saccade/blink events, synchronized EEG, and known text stimuli suitable for multimodal and stimulus-guided modeling.
