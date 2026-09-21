# NNDb-3T+

**Status:** Approved  
**Type:** Multimodal eye tracking and neuroimaging dataset  
**Paper publication date:** 2026-07-09  
**OpenNeuro dataset:** ds006642

## Summary

NNDb-3T+, the Naturalistic Neuroimaging Database 3T+, combines high frequency binocular eye tracking with 3 T fMRI during full length movie viewing and controlled sensory mapping tasks. It is particularly useful for naturalistic gaze modelling because the gaze stream can be synchronized to individual movie frames and scanner triggers.

## Eye tracking details

- **Eye tracker:** MRI compatible EyeLink 1000 Plus long range mount
- **Sampling rate:** 1000 Hz
- **Recording:** Binocular
- **Raw gaze trajectories:** Yes
- **Raw formats:** EDF and ASCII
- **Signals:** Continuous binocular gaze coordinates and pupil measurements
- **Eye movement event labels:** No dedicated ground truth fixation, saccade, microsaccade, or smooth pursuit label set was verified in the release documentation
- **Synchronization:** EyeLink message events allow alignment to scanner pulses, fMRI volumes, and individual movie frames

## Tasks and stimuli

### Movie watching

Participants watched the full movie *Back to the Future* across three runs while eye tracking and fMRI were recorded.

- **Task stimuli available:** **Partial**
- **Stimulus modality:** Full length movie
- **Movie included in dataset:** **No**
- **Reason:** Copyright restrictions prevent redistribution of the full movie
- **Synchronization support:** Movie frame numbers are embedded in the EyeLink ASCII stream, allowing precise alignment after the researcher obtains a legal copy of the movie

### Retinotopic mapping

Participants completed retinotopic mapping while maintaining fixation and responding to fixation dot colour changes.

- **Task stimuli available:** **Yes**
- **Stimulus materials and presentation scripts:** Included in the dataset's `stimuli/` directory

The dataset also includes somatotopic and tonotopic mapping tasks.

## Participants and scale

- **Participants:** 40
- **Naturalistic task:** Full length movie viewing
- **Controlled tasks:** Retinotopic, somatotopic, and tonotopic mapping
- **Eye tracking recorded during:** Movie viewing and retinotopic mapping

## Modalities

- Eye tracking
- 3 T fMRI
- Structural MRI
- Pulse oximetry
- Behavioural measures
- Cognitive assessments
- Questionnaire data

## Why it may be useful

NNDb-3T+ is especially interesting for future work involving:

- high frequency naturalistic gaze time series
- stimulus guided gaze representation learning
- gaze to video alignment
- multimodal eye tracking and fMRI modelling
- frame level visual context conditioning
- comparison between naturalistic and controlled viewing conditions

For stimulus guided modelling, the precise frame messages in the eye tracking stream are particularly valuable even though the copyrighted movie itself is not distributed.

## Caveats

The dataset should not currently be treated as a dedicated eye movement event benchmark because a separate ground truth fixation, saccade, or microsaccade annotation set was not verified.

The full *Back to the Future* movie is not distributed with the dataset. Researchers must obtain lawful access to the movie and follow the dataset's synchronization information when aligning it with gaze and fMRI.

The dataset documentation also notes a systematic playback onset delay affecting Run 3 of the movie watching session. Researchers should consult the supplied timing correction note before frame level alignment.

## Citation

Levchenko, E., Chow-Wing-Bom, H., Dick, F., Cooper, G., Tierney, A., & Skipper, J. I. (2026). A neuroimaging dataset combining movie-watching, eye-tracking, sensorimotor mapping, and cognitive tasks. *Scientific Data, 13*, 1184. https://doi.org/10.1038/s41597-026-07676-4

Dataset citation:

Levchenko, E., Chow-Wing-Bom, H., Dick, F., Tierney, A., & Skipper, J. I. (2026). Naturalistic Neuroimaging Database 3T+. OpenNeuro. https://doi.org/10.18112/openneuro.ds006642.v1.0.3

## Licence and attribution

- **Dataset licence:** CC BY 4.0
- Users should cite the associated Scientific Data paper and the OpenNeuro dataset when using the resource.
- The full movie is not covered for redistribution through the dataset and remains subject to its own copyright.

## Resources

- OpenNeuro dataset: https://openneuro.org/datasets/ds006642
- Dataset repository mirror: https://github.com/OpenNeuroDatasets/ds006642
- Scientific Data paper: https://doi.org/10.1038/s41597-026-07676-4
- Analysis and preprocessing code: https://github.com/levchenkoegor/movieproject2

## Catalog note

Added as an approved dataset because it provides raw 1000 Hz binocular gaze together with precise frame level stimulus synchronization and rich multimodal neuroimaging context.
