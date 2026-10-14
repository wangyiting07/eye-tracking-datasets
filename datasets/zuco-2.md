# ZuCo 2.0

**Status:** Approved  
**Type:** Multimodal eye tracking and EEG dataset  
**Original publication:** 2020  
**NEMAR BIDS release:** 2026-09-16

## Summary

ZuCo 2.0 extends the ZuCo resource with additional natural reading data and language-related tasks, combining 500 Hz eye tracking with 128-channel EEG. The 2026 NEMAR distribution provides a standardized BIDS-style archive with continuous gaze signals and eye-movement event metadata.

## Eye tracking details

- **Eye tracker:** EyeLink 1000
- **Sampling rate:** 500 Hz
- **Raw gaze trajectories:** Yes
- **Event annotations:** Fixations, saccades, and blinks
- **Microsaccade labels:** Not reported as a dedicated annotation set
- **Smooth pursuit labels:** Not applicable to the reading paradigm
- **Pupil information:** Included in the continuous eye tracking recordings

## Participants and task

- **Participants:** 18
- **Tasks:** Natural sentence reading and relation-extraction / annotation-related reading paradigms
- Eye tracking and EEG were recorded synchronously.

## Task stimuli

- **Task stimuli available:** **Yes**
- **Stimulus modality:** Text / sentences
- **Stimulus access:** Sentence materials are represented in the dataset/task files and associated metadata
- **Why this matters:** The displayed text can be aligned with gaze trajectories and EEG, supporting stimulus-guided multimodal modeling

## Modalities

- Eye tracking
- 128-channel EEG

## Why it may be useful

ZuCo 2.0 is particularly relevant for:

- gaze-aware language models
- multimodal text, gaze, and EEG representation learning
- fixation and saccade modeling during reading
- cognitive NLP
- stimulus-guided foundation models where the linguistic stimulus is directly available

Its combination of explicit text stimuli, high-frequency gaze, and neural signals is especially attractive for models that learn eye-movement dynamics conditioned on the content being viewed.

## 2026 update

The noteworthy 2026 change is the NEMAR-hosted BIDS-formatted release, which standardizes the archive structure, continuous gaze streams, and eye-movement event metadata for easier reuse.

## Citation

Hollenstein, N., Troendle, M., Zhang, C., & Langer, N. (2020). ZuCo 2.0: A dataset of physiological recordings during natural reading and annotation. In *Proceedings of the 12th Language Resources and Evaluation Conference (LREC 2020)*, 138–146. https://aclanthology.org/2020.lrec-1.18/

## Licence and attribution

Use of the dataset should follow the licence and citation terms listed by the official ZuCo / NEMAR distribution.

This repository does not redistribute the recordings or sentence materials. Users should verify the current archive licence and any upstream text-source restrictions before redistribution.

## Resources

- NEMAR dataset: https://www.nemar.org/dataset/nm000279
- Original paper: https://aclanthology.org/2020.lrec-1.18/

## Catalog note

Added as an approved dataset because it provides public 500 Hz raw gaze, fixation/saccade/blink events, synchronized EEG, and directly usable text stimuli for multimodal and stimulus-guided modeling.
