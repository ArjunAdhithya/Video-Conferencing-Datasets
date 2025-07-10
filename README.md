## Datasets for Video Conferencing

---

### Video Conferencing-Specific Datasets

#### 1. **Microsoft Video Conferencing Dataset (VCD)**  
- **Purpose**: Codec evaluation in realistic video conferencing settings  
- **Content**: 160 clips in 4 conferencing scenarios  
- **Modality**: Video only  
- **Access**: [GitHub – VCD](https://github.com/microsoft/VCD)  
- **Strengths**: Real-world conferencing conditions, camera variation  
- **Limitations**: Not focused on deepfakes or security analysis

#### 2. **Microsoft Video Call MOS Dataset**  
- **Purpose**: Predict perceived video quality in video calls  
- **Content**: 10 reference + 1,467 degraded Teams videos under 83 network conditions  
- **Modality**: Video (w/ transmission artifacts)  
- **Access**: [GitHub – Video_Call_MOS](https://github.com/microsoft/Video_Call_MOS)  
- **Strengths**: Real-world transmission degradation modeling  
- **Limitations**: No deepfake manipulations or annotations

#### 3. **Zoom-DF Dataset**  
- **Purpose**: Motion-based deepfake detection for conferencing  
- **Content**: Small set of synthetic Zoom-style clips  
- **Modality**: Video only  
- **Access**: By request (form submission) [paper](https://dl.acm.org/doi/abs/10.1145/3494109.3527195) 
- **Strengths**: Head/hand movement fakes, realistic Zoom context  
- **Limitations**: Very limited size, no facial blend fakes

---

### Foundational Deepfake Datasets

#### 4. **FaceForensics++**  
- **Purpose**: Benchmark for face manipulation detection  
- **Content**: 5,000 videos (1,000 real + 4,000 fakes) using 4 techniques  
- **Modality**: Video  
- **Access**: [FaceForensics++](https://github.com/ondyari/FaceForensics)  
- **Strengths**: Segmentation masks, multiple techniques  
- **Limitations**: Movie-style source videos, older synthesis

#### 5. **DFDC (DeepFake Detection Challenge)**  
- **Purpose**: Large-scale challenge benchmark  
- **Content**: 128,154 videos (23.6K real, 104.5K fake)  
- **Modality**: Video, Audio  
- **Access**: [Kaggle – DFDC](https://www.kaggle.com/competitions/deepfake-detection-challenge/data)  
- **Strengths**: Large, actor diversity, synthetic voice fakes included  
- **Limitations**: Controlled setting, coarse audio labeling

#### 6. **DeeperForensics-1.0**  
- **Purpose**: Realistic perturbation testing  
- **Content**: 59,475 videos (48.4K real, 11K fake)  
- **Modality**: Video  
- **Access**: Direct from official website [github](https://github.com/EndlessSora/DeeperForensics-1.0)
- **Strengths**: Real-world conditions simulated (compression, blur, lighting)  
- **Limitations**: One deepfake generation pipeline (DF-VAE)

#### 7. **ForgeryNet**  
- **Purpose**: Face forgery detection & localization  
- **Content**: 221,247 videos + 2.9M images across 15 manipulation types  
- **Modality**: Video, Image  
- **Access**: [Google Drive – ForgeryNet](https://github.com/DeviantArt/ForgeryNet)  
- **Strengths**: Multi-modal, multi-type, annotated  
- **Limitations**: Computationally large, movie-style clips

---
### Multimodal Datasets (Audio + Video)

#### 8. **FakeAVCeleb**  
- **Purpose**: Audio-video synchronization fakes  
- **Content**: 20,000 videos (500 real, 19.5K fake) with cloned voices  
- **Modality**: Audio + Video  
- **Access**: [Kaggle – FakeAVCeleb](https://www.kaggle.com/datasets/mohamedali262/fakeavceleb)  
- **Strengths**: Face + voice manipulation, celebrity diversity  
- **Limitations**: Non-conferencing content (celebrity interviews)

#### 9. **DeepSpeak**  
- **Purpose**: Webcam-style talking-head multimodal deepfakes  
- **Content**: ~13K videos (6.2K real, 6.7K fake); ~100 hours  
- **Modality**: Audio + Video  
- **Access**: [HuggingFace – DeepSpeak](https://huggingface.co/datasets/crestylab/deepspeak)  
- **Strengths**: Static camera setup, current generation fakes  
- **Limitations**: Scripted prompts, license agreement required

#### 10. **LAV-DF**  
- **Purpose**: Localized (partial) audio-video forgeries  
- **Content**: 100K+ video clips  
- **Modality**: Audio + Video  
- **Access**: [HuggingFace – LAV-DF](https://huggingface.co/datasets/LAV-DF)  
- **Strengths**: Segment-wise manipulation, sync error detection  
- **Limitations**: Limited to sync errors, license restricted

---

### Specialized / Real-World Deepfakes

#### 11. **Deepfake-Eval-2024**  
- **Purpose**: Real-world internet deepfake archive  
- **Content**: 45h video, 56.5h audio, 1,975 images  
- **Modality**: Audio + Video + Image  
- **Access**: Research request or paper link  
- **Strengths**: Real fakes from 88 websites, multilingual  
- **Limitations**: Copyright-sensitive, request-only

#### 12. **KoDF (Korean DeepFake)**  
- **Purpose**: Korean language and demographic inclusion  
- **Content**: 237,942 videos (62K real, 175K fake)  
- **Modality**: Video  
- **Access**: Request form (Google or AIHub)  
- **Strengths**: Scale, language diversity  
- **Limitations**: Demographic-specific, restricted access

#### 13. **WildDeepfake**  
- **Purpose**: Online-sourced deepfake analysis  
- **Content**: 7,314 clips from 707 videos  
- **Modality**: Video (faces only)  
- **Access**: [GitHub – WildDeepfake](https://github.com/deepfake-inthewild/wilddeepfake-dataset)  
- **Strengths**: Real-world fakes, in-the-wild  
- **Limitations**: Limited to face crops, small dataset

---

### Audio-Only Deepfake Datasets

#### 14. **ASVspoof (2019/2021)**  
- **Purpose**: Audio-only spoofing benchmark  
- **Content**: 10K–100K+ audio samples  
- **Modality**: Audio  
- **Access**: [Official site – ASVspoof](https://www.asvspoof.org/)  
- **Strengths**: Diverse TTS/VC attacks, large scale  
- **Limitations**: No video or conferencing content

#### 15. **WaveFake**  
- **Purpose**: Multilingual audio spoof dataset  
- **Content**: 134,000 fake utterances (English, Japanese)  
- **Modality**: Audio  
- **Access**: [Zenodo or Kaggle – WaveFake](https://zenodo.org/record/5773843)  
- **Strengths**: Multi-language, multiple TTS models  
- **Limitations**: Audio-only

---
### Dataset Table: All Datasets

| Dataset Name           | Modality         | Size / Duration                | Access Status      | Year | Conferencing Relevance | Link |
|------------------------|------------------|--------------------------------|---------------------|------|--------------------------|------|
| Microsoft VCD          | Video            | 160 clips                      | Active (GitHub)     | 2021 | Yes                      | [Link](https://github.com/microsoft/VCD) |
| Video Call MOS         | Video            | 1,467 degraded clips           | Active (GitHub)     | 2022 | Yes                      | [Link](https://github.com/microsoft/Video_Call_MOS) |
| Zoom‑DF                | Video            | Small Zoom-style fakes         | Request Required    | 2023 | Yes                      | [Paper](https://dl.acm.org/doi/abs/10.1145/3494109.3527195) |
| FaceForensics++        | Video            | 5,000 clips                    | Active (GitHub)     | 2019 | No                       | [Link](https://github.com/ondyari/FaceForensics) |
| DFDC                   | Video + Audio    | 128K videos (104K fake)        | Active (Kaggle)     | 2020 | No                       | [Link](https://www.kaggle.com/competitions/deepfake-detection-challenge/data) |
| DeeperForensics-1.0    | Video            | 59K videos                     | Request Required    | 2020 | No                       | [Link](https://github.com/EndlessSora/DeeperForensics-1.0) |
| ForgeryNet             | Video + Image    | 221K videos + 2.9M images      | Active (Google Drive) | 2021 | No                    | [Link](https://github.com/DeviantArt/ForgeryNet) |
| FakeAVCeleb            | Video + Audio    | 20K videos                     | Active (Kaggle)     | 2022 | Indirect                 | [Link](https://www.kaggle.com/datasets/mohamedali262/fakeavceleb) |
| DeepSpeak              | Video + Audio    | ~13K videos (~100h)            | Active (HuggingFace)| 2023 | Yes                      | [Link](https://huggingface.co/datasets/crestylab/deepspeak) |
| LAV-DF                 | Video + Audio    | 100K+ clips                    | Active (HuggingFace)| 2023 | Indirect                 | [Link](https://huggingface.co/datasets/LAV-DF) |
| Deepfake-Eval-2024     | Video + Audio + Image | 45h video, 56.5h audio, 1,975 images | Request Required | 2024 | Indirect            | [Link](https://github.com/BAAI-Open/Deepfake-Eval) |
| KoDF                   | Video            | 237K videos                    | Request Required    | 2021 | Indirect                 | [Link](https://github.com/nclab/KDF) |
| WildDeepfake           | Video            | 7,314 clips from online videos | Active (GitHub)     | 2020 | Indirect                 | [Link](https://github.com/deepfake-inthewild/wilddeepfake-dataset) |
| DF-Wild (UMD)          | Video            | ~48h of YouTube-style videos   | Active (GitHub)     | 2021 | Yes                      | [Link](https://github.com/granite-datasets/df-wild) |
| ASVspoof 2019/2021     | Audio            | 10K–100K+ clips                | Request Required    | 2019/21 | No                   | [Link](https://www.asvspoof.org/) |
| WaveFake               | Audio            | 134K utterances                | Active (Zenodo)     | 2021 | No                       | [Link](https://zenodo.org/record/5773843) |
| AVCAffe                | Video + Audio    | Cognitive load in calls        | Request Required    | 2022 | Yes                      | [Link](https://zenodo.org/record/6464358) |
| EasyPortrait           | Video (Face)     | Real-time portrait detection   | Active (GitHub)     | 2022 | Yes                      | [Link](https://github.com/deforum/easyportrait) |

---

### Focused Table: Video Conferencing–Related Datasets

| Dataset Name       | Modality      | Access Status     | Year | Conferencing Focus         |
|--------------------|---------------|-------------------|------|-----------------------------|
| Microsoft VCD      | Video         | Active (GitHub)   | 2021 | Real-world webcam calls     |
| Video Call MOS     | Video         | Active (GitHub)   | 2022 | Teams with degradation      |
| Zoom‑DF            | Video         | Request Required  | 2023 | Motion-based Zoom fakes     |
| DeepSpeak          | Audio + Video | Active (HF)       | 2023 | Webcam-style talking heads  |
| DF-Wild (UMD)      | Video         | Active (GitHub)   | 2021 | In-the-wild conferencing    |
| AVCAffe            | Video + Audio | Request Required  | 2022 | Cognitive load in meetings  |
| EasyPortrait       | Video (Face)  | Active (GitHub)   | 2022 | Face Parsing & Portrait Segmentation |

---
