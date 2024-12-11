# AUSpeech Dataset

## Overview
The AUSpeech dataset is a comprehensive multimodal database aimed at advancing research in Mandarin speech production. It includes synchronized ultrasound tongue imaging (UTI), audio recordings, and text annotations, providing a rich resource for linguistics, speech recognition, and clinical applications. This dataset features contributions from 43 healthy participants and 11 patients with dysarthria.

---


## Dataset Access and Download

### Access
The AUSpeech dataset is available for download at:  
[Dowload this datasets](https://1drv.ms/f/c/23457fe3d550acd1/Eq4JtIrnh4lJiBEz2KPyFM8BUq0FqjIr7LT8x5zQX810iw?e=AL9cLd)

### Size
The dataset size is approximately **700 GB**, including all audio, ultrasound, and text data.

### Usage Guidelines
- Ensure ethical use of the data for research and educational purposes.
- Cite the dataset appropriately in any publications or presentations.

---

## Dataset Structure


### Key Features and Corpus
- **High-resolution Ultrasound Imaging**: 920×700 pixels at 60 frames per second.
- **Multimodal Data**: Includes ultrasound, audio, and text annotations.
- **Extensive Speech Tasks**:
  - **Monophthongs**: Sustained pronunciation of 6 Mandarin vowels.
  - **Monosyllables**: Coverage of 405 distinct syllables.
  - **Sentences**: 375 unique sentences per participant, representing diverse Mandarin phonetic structures.
- **Participant Diversity**: Covers normal speakers from northern and southern China, with balanced gender representation.


### Participant Demographics
- **Healthy Participants**: 21 males, 22 females, average age: 24.2 years.
- **Dysarthria Patients**: 9 males, 2 females, age range: 45–70 years.
- **Total Participants**: 54 individuals.

### Data Structure and Organization
The dataset is organized into directories based on participants, with separate folders for each session. Data for each participant is divided into: 


1. **Audio Data**: Stored in `.wav` format (16 kHz sampling rate, mono-channel).
2. **Ultrasound Imaging Data**: Stored in `.dcm` format.
3. **Text Annotations**: Stored in `.lab` and `.TextGrid` formats for precise alignment.

### File Naming Convention
The files follow a consistent naming format:

**Example**: `speaker00012_M_s1_stn00001.wav`  
This format allows easy identification of the speaker, gender, session, and task.

---

## Data Collection Process

### Sessions
1. **Normal Session**:
   - Includes swallowing actions, monophthongs, monosyllables, and sentence tasks.
   - Designed to capture a wide range of articulatory behaviors.
2. **Patient Session**:
   - Focused on monophthongs monosyllables and words.
   - Adjustments were made for participants with speech and motor difficulties.

### Speech Tasks
- **Swallowing Actions**: Three swallows were recorded at the start and end of each session to ensure proper alignment and data segmentation.
- **Monophthongs**: Six Mandarin vowels (`/a/, /o/, /e/, /i/, /u/, /ü/`) were sustained for approximately two seconds each to capture stable imaging of tongue movement.
- **Monosyllables**: Participants were asked to produce 15 monosyllables from a pool of 405 commonly used syllables, covering diverse Mandarin phonetic patterns.
- **Sentences**: Each participant produced 375 unique sentences sourced from the Chinese Linguistic Data Consortium (CLDC), ensuring broad phonetic and syntactic diversity.

---

## Dataset Features

### Ultrasound Tongue Imaging
- High resolution: **920×700 pixels**.
- Captured at 60 frames per second.
- Dynamic range: **114 dB**.
- Probe setup: Sagittal placement under the chin with a custom support system to ensure stability.

### Audio Data
- Sampling rate: **16 kHz**.
- Format: Single-channel `.wav` files.

### Text Data
- Includes `.lab` and TextGrid files.
- Provides precise alignment between speech audio and ultrasound imaging.

---

## Applications

### Research
- **Phonetics and Linguistics**: Study Mandarin tones, articulation patterns, and the dynamics of tongue movements.
- **Speech Recognition and Synthesis**: Develop ultrasound-based ASR models and enhance synthesis systems.
- **Clinical Studies**: Analyze articulatory differences between healthy individuals and patients with dysarthria.

### Clinical Applications
- Speech therapy and rehabilitation for individuals with speech disorders.
- Development of AI-powered tools for speech assessment and education.

### Educational Use
- Training materials for teaching Mandarin as a second language.
- Resources for understanding Mandarin phonology and articulatory dynamics.


---


## Technical Validation


### Quality Assurance
- **Data Screening**: Frames with signal loss or motion artifacts were identified and removed using automated algorithms and manual review.
- **Consistency Checks**: Temporal alignment and imaging consistency were validated to ensure high data quality.

### Alignment
The Montreal Forced Aligner (MFA) was used to generate TextGrid files for accurate synchronization of speech audio and ultrasound imaging.
(We alignment using MFA on normal subject data and then conduct manual labeling checks. For patient data, we use manual annotation for audio pronunciation labeling.)
---

## Citation

If you use the AUSpeech dataset in your research, please cite:  
[mask]
---

## Acknowledgments

This work was supported by:
- **National Natural Science Foundation of China**.
- **Shenzhen Science and Technology Program**.
- **Shenzhen Peacock Team Project**.

For detailed funding information, refer to the official documentation.

---

## Contact Information
For questions or technical support regarding the dataset, please contact:  
yd.yang2@siat.ac.cn

Feel free to explore the AUSpeech dataset and leverage its rich resources for advancing research in speech science and clinical applications.
