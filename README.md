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
- **Access**: By request (form submission)  
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
- **Access**: Direct from official website  
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
## Dataset Comparison Table: All Datasets

| Dataset Name          | Modality            | Size / Duration                          | Access         | Key Purpose                                      |
|----------------------|---------------------|------------------------------------------|----------------|--------------------------------------------------|
| **VCD**              | Video               | 160 clips                                | GitHub         | Codec evaluation in conferencing settings        |
| **Video Call MOS**   | Video               | 1,467 degraded Teams videos              | GitHub         | Video call quality prediction                    |
| **Zoom-DF**          | Video               | Small synthetic Zoom-style clips         | Request Form   | Motion-based deepfake detection                  |
| **FaceForensics++**  | Video               | 5,000 videos (1,000 real + 4,000 fake)   | GitHub         | Classic facial manipulation benchmark            |
| **DFDC**             | Audio + Video       | 128K videos (104K fake)                  | Kaggle         | Large-scale deepfake detection challenge         |
| **DeeperForensics-1.0** | Video           | 59K videos (11K fake)                    | Official Site  | Perturbation-aware realism testing               |
| **ForgeryNet**       | Video + Image       | 221K videos + 2.9M images                | Google Drive   | Multi-type forgery detection and localization    |
| **FakeAVCeleb**      | Audio + Video       | 20K videos                               | Kaggle         | AV sync deepfakes using celebrity interviews     |
| **DeepSpeak**        | Audio + Video       | ~13K videos, ~100 hours total            | HuggingFace    | Webcam-style, multimodal, scripted recordings     |
| **LAV-DF**           | Audio + Video       | 100K+ clips                              | HuggingFace    | Partial/sync-manipulated forgeries               |
| **Deepfake-Eval-2024** | Audio + Video + Image | 45h video, 56.5h audio, 1,975 images | Request         | Real-world multilingual deepfakes                |
| **KoDF**             | Video               | 237K videos (175K fake)                  | Request Form   | Korean language deepfake repository              |
| **WildDeepfake**     | Video               | 7,314 clips from 707 online videos       | GitHub         | Uncontrolled real-world deepfakes                |
| **ASVspoof 2019/21** | Audio               | 10K–100K+ audio clips                    | Registration   | Audio spoofing (TTS/VC) benchmarks               |
| **WaveFake**         | Audio               | 134K utterances (EN & JP)                | Zenodo/Kaggle  | Multilingual audio deepfake detection            |

---

## Focused Dataset Table: Video Conferencing–Related Resources

| Dataset Name         | Modality         | Size / Duration               | Access        | Unique Focus                                        |
|----------------------|------------------|-------------------------------|---------------|-----------------------------------------------------|
| **VCD**              | Video            | 160 clips                     | GitHub        | Realistic webcam/meeting-style compression testing  |
| **Video Call MOS**   | Video            | 1,467 degraded videos         | GitHub        | Teams video with simulated network degradation      |
| **Zoom‑DF**          | Video            | Small synthetic Zoom-style set| Request Form  | Head/hand motion fakes in conferencing setup        |
| **DeepSpeak v1.0**   | Audio + Video    | ~13K videos, ~100h total      | HuggingFace   | Static talking-head webcam clips                    |
| **DF-Wild**          | Video            | ~7K clips (~48h video total)  | GitHub        | Web-conferencing-like videos from YouTube           |


---
