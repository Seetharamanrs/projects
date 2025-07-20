# Schwa Sound Identification in ESOL Learners

##  Project Overview
This project addresses a key challenge in ESOL (English for Speakers of Other Languages) education: accurately identifying and providing feedback on mispronunciations of the schwa sound — the most common yet often overlooked vowel sound in English. 

Traditional language feedback systems offer word-level corrections, which often miss finer, phoneme-level deviations that are crucial to fluency. This project implements an AI-powered speech analysis pipeline that focuses specifically on schwa-related phonetic features to deliver more precise, personalised feedback.

---

##  Problem Statement
ESOL learners frequently struggle with accurate pronunciation, particularly with the **schwa sound** (/ə/), which appears in unstressed syllables and varies subtly across contexts. Key issues include:

- **Lack of phoneme-level feedback** in conventional ESOL learning tools.
- **Limited teacher capacity** to offer consistent, detailed correction.
- **High variation in schwa usage** in British English, making it hard for learners to generalise rules.

---

##  Objective
To design a system that:
- Detects schwa sounds from learner speech.
- Extracts and analyzes acoustic properties like frequency, duration, intensity, and spectral shape.
- Provides **granular feedback** to help learners correct pronunciation at a phonetic level.

---

## Solution Approach

1. **Client Collaboration**  
   Worked directly with a client (21st Century Educators) in the ESOL space to understand user pain points and tailor the pipeline to real learner data.

2. **Audio Input & Preprocessing**  
   - Collected word-level speech recordings containing target schwa sounds.
   - Converted audio to waveforms using libraries like `Librosa`.

3. **Feature Extraction**  
   - Applied signal processing to isolate schwa-relevant features:
     - **Formant frequencies (F1, F2)**
     - **Duration of unstressed vowel**
     - **Spectral centroid and bandwidth**

4. **Analysis and Feedback Generation**  
   - Compared learner audio features to standard British English benchmarks.
   - Flagged deviations in schwa production for targeted feedback.

5. **Scalability & Modularity**  
   - Built a pipeline structure that allows extension to other phonemes and dialect variations.

---

## Why This Approach?
- **Granular phonetic feedback** empowers learners with specific, correctable targets.
- **AI-driven analysis** is scalable and consistent — unlike human-only feedback systems.
- Focus on the **schwa sound**, which is central to natural-sounding English but often ignored in typical ESOL systems.
  
---

##  Key Features
- Phoneme-level feedback for schwa recognition.
- Signal-based feature extraction and analysis.
- Modular pipeline design for easy extension.

---

##  Tech Stack & Skills Used

- **Languages:** Python  
- **Libraries:** Librosa, NumPy, SciPy, Matplotlib  
- **Skills:**  
  - Audio Signal Processing  
  - Speech Feature Extraction  
  - ESOL Linguistics & Phonetics  
  - AI-driven Feedback Systems  
  - Client-Focused Solution Design

---

## Future Work
- Integrate real-time feedback for classroom or app-based ESOL tools.
- Expand to other difficult phonemes (e.g., /θ/, /ð/, /r/).
- Incorporate multilingual comparison models for better transfer learning.

---
#  Acknowledgements

I would like to sincerely thank my client(21st Century Educators)  for giving me the opportunity to work on this project. Their guidance and support were invaluable in shaping a practical, real-world solution. This collaboration allowed me to apply technical and linguistic knowledge to a meaningful challenge in ESOL education.

## Contact
For questions or collaboration inquiries, feel free to reach out [mail](rseetharaman293@example.com)