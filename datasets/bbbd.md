# Brain, Body, and Behavior Dataset (BBBD)

**Status:** Approved  
**Type:** Multimodal eye tracking, neural, physiological, and behavioural dataset  
**Publication date:** 2026-04-21  
**Scientific Data article:** 13, 920 (2026)

## Summary

The Brain, Body, and Behavior Dataset (BBBD) contains approximately 110 hours of synchronized recordings from 178 participants across five experiments involving short educational videos. It combines eye tracking with EEG, EOG, ECG, respiration, head motion, behavioural measures, and participant-level cognitive and questionnaire data.

The dataset is especially relevant for multimodal representation learning because all released continuous signals are time-aligned to the educational video stimuli.

## Eye tracking details

- **Eye tracker:** EyeLink 1000 with 35 mm lens
- **Original acquisition rate:** 500 Hz
- **Public released sampling rate:** **128 Hz**
- **Raw gaze trajectories publicly available:** **Yes, but the released continuous gaze/pupil files are resampled to 128 Hz rather than untouched native 500 Hz streams**
- **Signals:** Gaze position, pupil size, head position
- **Event annotations:** Fixations, saccades, and blinks
- **Microsaccade labels:** Not reported as a dedicated annotation set
- **Smooth pursuit labels:** Not reported

Blinks and saccades were detected using the eye tracker's event-detection algorithm. The public release standardizes continuous signals to 128 Hz across modalities.

## Participants and scale

- **Participants analyzed:** 178
- **Experiments:** 5
- **Approximate total recording duration:** 110 hours
- **Video exposure:** 3 to 6 educational videos per participant
- **Mean viewing duration:** approximately 28 minutes per participant

## Tasks and stimuli

Participants watched short educational videos under conditions including attentive viewing, distraction, differing learning goals, and motivational manipulations.

- **Task stimuli available:** **Partial / externally available**
- **Stimulus modality:** Educational videos
- **Number of unique videos:** 11
- **Stimulus access:** The paper and experiment README files provide the source YouTube URLs
- **Synchronization:** All released signals are aligned to video onset and offset
- **Stimulus files redistributed in the dataset:** Not treated here as bundled redistributable media; users should follow the original video source and copyright terms

This makes BBBD particularly useful for stimulus-guided models that combine visual/video information with gaze and neural or physiological time series.

## Modalities

- Eye tracking
- EEG
- EOG
- ECG
- Respiration
- Head motion
- Behavioural measures
- Quiz performance
- Engagement ratings
- ADHD self-report scores
- Working-memory measures

## Why it may be useful

BBBD is especially interesting for future work involving:

- multimodal foundation models combining gaze, EEG, and physiology
- stimulus-guided eye tracking representation learning
- educational-video understanding with synchronized gaze
- attention and engagement modelling
- cross-modal self-supervised learning
- learning from fixation, saccade, blink, pupil, and neural signals jointly

Its main strength for your future direction is the combination of synchronized stimulus information with several behavioural and physiological streams at participant scale.

## Important sampling-rate caveat

The EyeLink 1000 originally recorded gaze position, head position, and pupil size at **500 Hz**.

For the final public release, these continuous signals were resampled to the common **128 Hz** time base used across modalities. Therefore, this catalog records the dataset as:

> **128 Hz public release; 500 Hz original acquisition**

The publicly released continuous files should not be treated as untouched native-resolution 500 Hz EyeLink recordings.

## Citation

Madsen, J., Kuppa, N., & Parra, L. C. (2026). The Brain, Body, and Behavior Dataset (BBBD): Multimodal Recordings during Educational Videos. *Scientific Data, 13*, 920. https://doi.org/10.1038/s41597-026-07215-1

Dataset DOI:

https://doi.org/10.5281/zenodo.19241964

## Licence and attribution

Users should cite the Scientific Data article and follow the current licence and usage terms provided with the official Zenodo / INDI release.

The educational videos originate from external video sources. Their copyright and redistribution conditions are separate from the BBBD dataset itself and should be checked before reproducing or redistributing stimulus content.

## Resources

- Scientific Data paper: https://doi.org/10.1038/s41597-026-07215-1
- Zenodo dataset: https://doi.org/10.5281/zenodo.19241964
- INDI dataset: https://doi.org/10.15387/fcp_indi.retro.bbbd
- Code: https://github.com/madjens/bbbd-dataset

## Catalog note

Added as an approved dataset because it provides public multimodal time series, eye movement event annotations, identifiable educational stimuli, and strong synchronization across gaze, neural, physiological, and behavioural signals.
