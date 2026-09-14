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

## Task and stimuli

- **Task:** Free viewing of natural scenes for 4 seconds per scene, with verbal scene captioning on 25% of trials
- **Task stimuli available:** **Yes**
- **Stimulus modality:** Natural scene images
- **Stimulus set:** 4,080 scenes drawn from the Natural Scenes Dataset
- **Stimulus access:** The released AVS dataset includes the scene images in the `stimuli/` directory
- **Additional stimulus information:** COCO and COCO-Stuff annotations and a scene image licence table are provided

The task stimuli are therefore directly usable together with the gaze data, which makes AVS particularly attractive for future models that use visual stimulus information to guide representation learning from eye movements.

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
- **the actual visual stimuli used in the task**
- synchronized neurophysiology
- semantic labels at the fixation level

This makes it useful for future work on multimodal gaze modelling, eye movement representation learning, gaze conditioned visual models, stimulus guided eye tracking models, and analyses of the relationship between eye movements, visual content, and neural responses.

## Citation

If you use AVS in research, cite the official dataset paper:

Sulewski, P., Amme, C., König, P., Hebart, M. N., & Kietzmann, T. C. (2026). *Active Visual Semantics: A large-scale MEG and eye-tracking dataset for understanding visual intelligence in action*. arXiv:2609.01055 [q-bio.NC]. https://doi.org/10.48550/arXiv.2609.01055

The AVS documentation notes that this is currently a preprint and that the citation should be updated if a peer-reviewed version with a different venue or DOI becomes available.

Because the AVS stimulus set was drawn from the Natural Scenes Dataset, the NSD source should also be acknowledged when relevant:

Allen, E. J., St-Yves, G., Wu, Y., et al. (2022). *A massive 7T fMRI dataset to bridge cognitive neuroscience and artificial intelligence*. Nature Neuroscience, 25, 116–126. https://doi.org/10.1038/s41593-021-00962-x

## Licence and attribution

- **AVS dataset licence:** Creative Commons Attribution 4.0 International, CC BY 4.0
- **Attribution:** The AVS dataset paper above should be cited when the dataset is used
- **Software:** pyAVS is distributed separately and its own repository/licence should be consulted if the software is reused
- **Stimulus images:** The 4,080 scene images originate from NSD and ultimately from MS COCO. They retain upstream image-specific licences rather than automatically inheriting the AVS dataset licence
- **Before reproducing or redistributing stimulus images:** Check the released `stimuli/avs_scenes_all_licenses.parquet` licence table and the applicable upstream terms

This catalog entry does not redistribute AVS data or stimulus images. It only summarizes the resource and links to the official sources.

## Caveats

The dataset should not currently be treated as a dedicated microsaccade benchmark. Saccades are annotated, but a separate microsaccade label set was not clearly documented in the release information reviewed when this entry was created.

The scene images originate from the Natural Scenes Dataset and retain their upstream licences. The AVS release provides a licence table that should be checked before redistribution or publication of stimulus images.

## Resources

- Dataset documentation: https://www.kietzmannlab.uni-osnabrueck.de/avs/
- Official citation page: https://www.kietzmannlab.uni-osnabrueck.de/avs/reference/citation.html
- Data access documentation: https://www.kietzmannlab.uni-osnabrueck.de/avs/data_access.html
- AWS Open Data registry: https://registry.opendata.aws/avs/
- Dataset paper: https://arxiv.org/abs/2609.01055
- Public data access is provided through the AVS AWS Open Data release

## Catalog note

Added to this repository as a potentially useful future research dataset because it provides raw high frequency gaze data, event annotations, the original task stimuli, and rich multimodal context.
