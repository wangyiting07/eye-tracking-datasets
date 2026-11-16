# Naturalistic Smartphone Interaction Multimodal Dataset

**Status:** Approved  
**Type:** Multimodal eye tracking, EEG, and physiological dataset  
**Publication date:** 2026-11-11  
**OpenNeuro dataset:** ds007537

## Summary

This dataset combines wearable eye tracking with 64-channel EEG, PPG, and GSR during naturalistic smartphone interaction followed by a standardized relaxation period. It is useful for studying attention, engagement, physiological state, and multimodal representations during realistic screen use.

## Eye tracking details

- **Eye tracker:** Tobii Pro Glasses 2
- **Exact released gaze sampling rate:** **Not yet verified from the public BIDS sidecar**
- **Continuous sample-level gaze publicly available:** **Yes**
- **Original Tobii source format described by the paper:** `livedata.json.gz`
- **Public format:** BIDS-compatible compressed TSV tables, including files such as `*_recording-cyclopean_physio.tsv.gz`
- **Public gaze fields:** timestamps, 2D gaze coordinates, 3D gaze points, gaze-direction vectors, pupil size, and pupil-center positions
- **Fixation labels:** No dedicated released annotation set verified
- **Saccade labels:** No dedicated released annotation set verified
- **Microsaccade labels:** Not reported
- **Smooth pursuit labels:** Not reported

The public release therefore contains continuous eye-tracking samples suitable for time-series modeling, even though the exact gaze sampling frequency still needs to be confirmed from the dataset-specific metadata rather than inferred from the Tobii device specification.

## Participants and protocol

- **Participants reported in the paper:** 30
- **Naturalistic smartphone phase:** approximately 10 minutes
- **Relaxation phase:** approximately 5 minutes
- Smartphone use included naturalistic activities such as gaming or short-form video viewing.
- The relaxation phase used a standardized nature video.
- Hardware markers were used for session synchronization, with additional periodic markers during recording.

## Task stimuli

- **Task stimuli available:** **Partial / mixed**
- **Naturalistic smartphone content:** Participant-dependent rather than one fixed stimulus set
- **Relaxation stimulus:** Standardized nature video
- **Stimulus modality:** Smartphone visual content and video
- **Stimulus packaging:** The smartphone content should not be treated as a single fully reproducible distributed stimulus set

For future stimulus-guided modeling, this dataset is therefore more useful for learning from realistic screen-use context than for exact frame-matched stimulus reconstruction across all participants.

## Modalities

- Eye tracking
- 64-channel EEG
- PPG
- GSR

## Why it may be useful

This dataset is particularly relevant for:

- multimodal attention and engagement modeling
- eye tracking + EEG representation learning
- physiological modeling during naturalistic smartphone use
- screen-use and short-video research
- self-supervised multimodal learning from gaze, neural, and autonomic signals
- studying state changes between active smartphone interaction and relaxation

## Limitations

The exact public eye-tracking sampling rate has not yet been verified from the released BIDS JSON sidecar, so this catalog deliberately does **not** label it as 50 Hz solely from the Tobii Pro Glasses 2 device specification.

No dedicated ground-truth fixation, saccade, microsaccade, or smooth-pursuit annotation set has been verified.

Naturalistic smartphone content varies between participants, limiting precise stimulus-level reproducibility compared with datasets such as AVS, ZuCo, or NNDb-3T+.

## Citation

Mishra, Gandhi, Gandhi, et al. (2026). A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions. *Scientific Data*. https://doi.org/10.1038/s41597-026-08615-z

## Licence and attribution

Users should cite the Scientific Data article and follow the current licence and usage terms provided with the official OpenNeuro release.

Any third-party smartphone content or video material remains subject to its original copyright and usage terms and should not be assumed to be redistributable under the dataset's own licence.

## Resources

- Scientific Data paper: https://doi.org/10.1038/s41597-026-08615-z
- OpenNeuro dataset: https://openneuro.org/datasets/ds007537
- EEGDash metadata: https://eegdash.org/api/dataset/eegdash.dataset.ON007537.html

## Catalog note

Added as an approved dataset because it provides public continuous sample-level gaze together with EEG, PPG, and GSR during naturalistic smartphone interaction. The eye-tracking sampling rate remains intentionally marked as unverified until confirmed from the released sidecar metadata.
