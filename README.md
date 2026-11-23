# Awesome Audio-Video Unification

<p align="center">
  <a href="https://hkust.edu.hk/"><img src="src/hkust.svg" alt="HKUST" width="150"></a>
  &emsp;
  <a href="https://cqf.io/lab.html"><img src="src/hkust-visual-intelligence-lab.png" alt="Visual Intelligence Lab at HKUST" width="175"></a>
  &emsp;
  <a href="https://long-group.cse.ust.hk/"><img src="src/hkust-long-group.png" alt="LONG Group at HKUST" width="145"></a>
</p>

## ✨ Survey Highlights

> How do models understand sounding video, generate it, and combine both abilities?

- **Unifying Audio-Video Understanding and Generation: Foundations, Taxonomies, and Architectures**  
  Kien T. Pham · Zhenqi He · Yanghao Wang · Qifeng Chen · Long Chen  
  [📖 Survey](paper/arxiv.pdf) · [🗂️ Complete Taxonomy](src/taxonomy_complete.png) · [✒️ BibTeX](#bibtex)
- **Three research pillars:** [Generation](#audio-video-generation) synthesizes one or both streams; [Understanding](#audio-video-understanding) interprets their joint content; [Unified Architectures](#unified-architectures) connect perception and synthesis.
- **Shared foundations:** [Tokenization](#audio-video-tokenization), [Datasets](#awesome-datasets), and [Evaluation](#awesome-benchmarks-and-metrics) cover the representations, training data, and protocols used across those pillars.

<p align="center">
  <img src="src/three_pillars_integration.png" alt="The three research pillars and the semantic, temporal, and spatial alignment axes" width="90%">
</p>

[Generation Timeline](src/av_generation_timeline.png) · [Understanding Timeline](src/understanding_timeline.png) · [Unification Timeline](src/unification_timeline.png) · [BibTeX Library](src/references.bib)

---

## Table of Contents

<!-- contents:start -->
- [Awesome Papers](#awesome-papers)
  - [Audio-Video Generation](#audio-video-generation)
    - [Video-to-Audio (V2A)](#video-to-audio-v2a)
    - [Audio-to-Video (A2V)](#audio-to-video-a2v)
    - [Joint Audio-Video Generation](#joint-audio-video-generation)
  - [Audio-Video Understanding](#audio-video-understanding)
    - [Task-Specific Models](#task-specific-models)
    - [Self-Supervised Learning](#self-supervised-learning)
    - [MLLM Generalists](#mllm-generalists)
  - [Unified Architectures](#unified-architectures)
    - [Fully Autoregressive](#fully-autoregressive)
    - [Fully Diffusion](#fully-diffusion)
    - [Decoupled Hybrid](#decoupled-hybrid)
    - [Modular / Agentic](#modular--agentic)
  - [Audio-Video Tokenization](#audio-video-tokenization)
    - [Audio Tokenizers](#audio-tokenizers)
    - [Video Tokenizers](#video-tokenizers)
    - [Joint Audio-Video Tokenization](#joint-audio-video-tokenization)
- [Awesome Datasets](#awesome-datasets)
  - [Joint Audio-Video Corpora](#joint-audio-video-corpora)
  - [Video Pretraining](#video-pretraining)
  - [Audio Pretraining](#audio-pretraining)
- [Awesome Benchmarks and Metrics](#awesome-benchmarks-and-metrics)
  - [Benchmarks](#benchmarks)
  - [Metrics](#metrics)
- [Related Work and Foundations](#related-work-and-foundations)
- [Acknowledgements](#acknowledgements)
- [BibTeX](#bibtex)
<!-- contents:end -->

The catalog covers all 354 references cited in the survey. Each taxonomy leaf gets one table, ordered newest to oldest by the survey’s bibliography year, with titles used to break ties. A work can appear in multiple roles. Titles link to the paper or, for releases without a paper, the release documentation. A dash in Resources means no resource link was confirmed, not necessarily that none exists. A GitHub link labeled **GitHub** rather than **Code** points to a companion repository, not a released implementation.

---

<!-- catalog:start -->
## Awesome Papers

### Audio-Video Generation

#### Video-to-Audio (V2A)

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Audio-Omni: Extending Multi-modal Understanding to Versatile Audio Generation and Editing**](<https://arxiv.org/abs/2604.10708>) | 2026 | arXiv | [Code](<https://github.com/ZeyueT/Audio-Omni>) · [Project](<https://zeyuet.github.io/Audio-Omni>) |
| [**AudioX: A Unified Framework for Anything-to-Audio Generation**](<https://openreview.net/forum?id=qjJWxK3yWo>) | 2026 | ICLR | [Code](<https://github.com/ZeyueT/AudioX>) · [Project](<https://zeyuet.github.io/AudioX/>) |
| [**MuMu-LLaMA: Multi-modal Music Understanding and Generation via Large Language Models**](<https://doi.org/10.1016/j.eswa.2025.130688>) | 2026 | Expert Systems with Applications | [Code](<https://github.com/shansongliu/MuMu-LLaMA>) · [Project](<https://crypto-code.github.io/MuMu-LLaMA_Demo/>) |
| [**UNISON: A Unified Sound Generation and Editing Framework via Deep LLM Fusion**](<https://arxiv.org/abs/2605.31530>) | 2026 | arXiv | [Code](<https://github.com/lizhaoqing/UNISON>) · [Models](<https://huggingface.co/jac22/UNISON>) |
| [**MMAudio: Taming Multimodal Joint Training for High-Quality Video-to-Audio Synthesis**](<https://openaccess.thecvf.com/content/CVPR2025/html/Cheng_MMAudio_Taming_Multimodal_Joint_Training_for_High-Quality_Video-to-Audio_Synthesis_CVPR_2025_paper.html>) | 2025 | CVPR | [Code](<https://github.com/hkchengrex/MMAudio>) · [Project](<https://hkchengrex.com/MMAudio/>) · [Demo](<https://huggingface.co/spaces/hkchengrex/MMAudio>) |
| [**Read, Watch and Scream! Sound Generation from Text and Video**](<https://arxiv.org/abs/2407.05551>) | 2025 | AAAI | [Code](<https://github.com/naver-ai/rewas>) · [Project](<https://naver-ai.github.io/rewas>) |
| [**Temporally aligned audio for video with autoregression**](<https://doi.org/10.1109/icassp49660.2025.10890587>) | 2025 | ICASSP | [Code](<https://github.com/ilpoviertola/v-aura>) |
| [**VinTAGe: Joint Video and Text Conditioning for Holistic Audio Generation**](<https://openaccess.thecvf.com/content/CVPR2025/html/Kushwaha_VinTAGe_Joint_Video_and_Text_Conditioning_for_Holistic_Audio_Generation_CVPR_2025_paper.html>) | 2025 | CVPR | — |
| [**Vmas: Video-to-music generation via semantic alignment in web music videos**](<https://arxiv.org/abs/2409.07450>) | 2025 | 2025 IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) | [Project](<https://genjib.github.io/project_page/VMAs/index.html>) |
| [**FoleyCrafter: Bring Silent Videos to Life with Lifelike and Synchronized Sounds**](<https://arxiv.org/abs/2407.01494>) | 2024 | arXiv | [Code](<https://github.com/open-mmlab/FoleyCrafter>) · [Project](<https://foleycrafter.github.io/>) · [Demo](<https://huggingface.co/spaces/ymzhang319/FoleyCrafter>) |
| [**Seeing and Hearing: Open-domain Visual-Audio Generation with Diffusion Latent Aligners**](<https://doi.org/10.1109/cvpr52733.2024.00683>) | 2024 | CVPR | [Code](<https://github.com/yzxing87/Seeing-and-Hearing>) |
| [**SonicVisionLM: Playing Sound with Vision Language Models**](<https://doi.org/10.1109/cvpr52733.2024.02537>) | 2024 | CVPR | — |
| [**V2A-Mapper: A Lightweight Solution for Vision-to-Audio Generation by Connecting Foundation Models**](<https://arxiv.org/abs/2308.09300>) | 2024 | AAAI | [Code](<https://github.com/heng-hw/V2A-Mapper>) |
| [**Diff-Foley: Synchronized Video-to-Audio Synthesis with Latent Diffusion Models**](<https://arxiv.org/abs/2306.17203>) | 2023 | NeurIPS | [Code](<https://github.com/luosiallen/Diff-Foley>) |
| [**I Hear Your True Colors: Image Guided Audio Generation**](<https://arxiv.org/abs/2211.03089>) | 2023 | ICASSP | [Code](<https://github.com/RoySheffer/im2wav>) · [Project](<https://pages.cs.huji.ac.il/adiyoss-lab/im2wav/>) |
| [**M$^2$UGen: Multi-modal Music Understanding and Generation with the Power of Large Language Models**](<https://arxiv.org/abs/2311.11255>) | 2023 | arXiv | [Code](<https://github.com/shansongliu/M2UGen>) |
| [**Taming Visually Guided Sound Generation**](<https://arxiv.org/abs/2110.08791>) | 2021 | BMVC | [Code](<https://github.com/v-iashin/SpecVQGAN>) · [Project](<http://v-iashin.github.io/SpecVQGAN>) |

#### Audio-to-Video (A2V)

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**FlowAct-R1: Towards Interactive Humanoid Video Generation**](<https://arxiv.org/abs/2601.10103>) | 2026 | arXiv | [Project](<https://grisoon.github.io/FlowAct-R1/>) |
| [**FlowAct-R2: Beyond Talking Avatar via Streaming Multimodal References and Proactive Agent Planning**](<https://arxiv.org/abs/2609.35728>) | 2026 | arXiv | [Project](<https://bone-11.github.io/Flowact-R2/>) · [Demo](<https://huggingface.co/spaces/ProAudience/FlowAct-R2>) |
| [**InteractiveAvatar: Real-Time Streaming Video Generation for Consistent and Intent-Aware Avatars**](<https://arxiv.org/abs/2606.22905>) | 2026 | arXiv | [Project](<https://sqymu.github.io/InteractiveAvatar/>) |
| [**A Simple but Strong Baseline for Sounding Video Generation: Effective Adaptation of Audio and Video Diffusion Models for Joint Generation**](<https://arxiv.org/abs/2409.17550>) | 2025 | arXiv | [Code](<https://github.com/sonyresearch/svg_baseline>) |
| [**Choreomuse: Robust music-to-dance video generation with style transfer and beat-adherent motion**](<https://arxiv.org/abs/2507.19836>) | 2025 | ACM MM | [Project](<https://choreomuse.github.io/>) |
| [**DiTalker: A Unified DiT-based Framework for High-Quality and Speaking Styles Controllable Portrait Animation**](<https://arxiv.org/abs/2508.06511>) | 2025 | arXiv | [Project](<https://thenameishope.github.io/DiTalker/>) |
| [**Hallo3: Highly Dynamic and Realistic Portrait Image Animation with Video Diffusion Transformer**](<https://arxiv.org/abs/2412.00733>) | 2025 | arXiv | [Code](<https://github.com/fudan-generative-vision/hallo3>) · [Project](<https://fudan-generative-vision.github.io/hallo3/>) |
| [**Live Avatar: Streaming Real-time Audio-Driven Avatar Generation with Infinite Length**](<https://arxiv.org/abs/2512.04677>) | 2025 | arXiv | [Code](<https://github.com/Alibaba-Quark/LiveAvatar>) · [Project](<https://liveavatar.github.io/>) |
| [**SpA2V: Harnessing Spatial Auditory Cues for Audio-driven Spatially-aware Video Generation**](<https://arxiv.org/abs/2508.00782>) | 2025 | ACM MM | — |
| [**Wan-S2V: Audio-Driven Cinematic Video Generation**](<https://arxiv.org/abs/2508.18621>) | 2025 | arXiv | — |
| [**YingVideo-MV: Music-Driven Multi-Stage Video Generation**](<https://arxiv.org/abs/2512.02492>) | 2025 | arXiv | [Code](<https://github.com/GiantAILab/YingVideo-MV>) · [Project](<https://giantailab.github.io/YingVideo-MV/>) |
| [**AniPortrait: Audio-Driven Synthesis of Photorealistic Portrait Animation**](<https://arxiv.org/abs/2403.17694>) | 2024 | arXiv | [Code](<https://github.com/scutzzj/aniportrait>) |
| [**Diverse and Aligned Audio-to-Video Generation via Text-to-Video Model Adaptation**](<https://ojs.aaai.org/index.php/AAAI/article/view/28486>) | 2024 | AAAI | — |
| [**EMO: Emote Portrait Alive -- Generating Expressive Portrait Videos with Audio2Video Diffusion Model under Weak Conditions**](<https://arxiv.org/abs/2402.17485>) | 2024 | arXiv | — |
| [**Hallo: Hierarchical Audio-Driven Visual Synthesis for Portrait Image Animation**](<https://arxiv.org/abs/2406.08801>) | 2024 | arXiv | [Code](<https://github.com/fudan-generative-vision/hallo>) · [Project](<https://fudan-generative-vision.github.io/hallo/#/>) · [Data](<https://huggingface.co/datasets/fudan-generative-ai/hallo_inference_samples>) |
| [**Real3D-Portrait: One-shot Realistic 3D Talking Portrait Synthesis**](<https://arxiv.org/abs/2401.08503>) | 2024 | ICLR | [Code](<https://github.com/yerfor/Real3DPortrait>) · [Project](<https://real3dportrait.github.io>) |
| [**Seeing and Hearing: Open-domain Visual-Audio Generation with Diffusion Latent Aligners**](<https://doi.org/10.1109/cvpr52733.2024.00683>) | 2024 | CVPR | [Code](<https://github.com/yzxing87/Seeing-and-Hearing>) |
| [**V-Express: Conditional Dropout for Progressive Training of Portrait Video Generation**](<https://arxiv.org/abs/2406.02511>) | 2024 | arXiv | [Code](<https://github.com/tencent-ailab/V-Express>) · [Project](<https://tenvence.github.io/p/v-express/>) |
| [**WorldGPT: Empowering LLM as Multimodal World Model**](<https://openreview.net/forum?id=G1tsqarGAw>) | 2024 | ACM MM | — |
| [**SadTalker: Learning Realistic 3D Motion Coefficients for Stylized Audio-Driven Single Image Talking Face Animation**](<https://arxiv.org/abs/2211.12194>) | 2023 | CVPR | [Code](<https://github.com/winfredy/sadtalker>) |
| [**The Power of Sound (TPoS): Audio Reactive Video Generation with Stable Diffusion**](<https://arxiv.org/abs/2309.04509>) | 2023 | arXiv | [Project](<https://ku-vai.github.io/TPoS/>) |
| [**Sound2Sight: Generating Visual Dynamics from Sound and Context**](<https://doi.org/10.1007/978-3-030-58583-9_42>) | 2020 | ECCV | — |

#### Joint Audio-Video Generation

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Apollo: Unified Multi-Task Audio-Video Joint Generation**](<https://arxiv.org/abs/2601.04151>) | 2026 | arXiv | — |
| [**Introducing Pika H3 Flex**](<https://pika.art/blog/pika-h3-flex>) | 2026 | — | — |
| [**JavisDiT++: Unified Modeling and Optimization for Joint Audio-Video Generation**](<https://arxiv.org/abs/2602.19163>) | 2026 | ICLR | [Code](<https://github.com/JavisVerse/JavisDiT>) · [Project](<https://javisverse.github.io/JavisDiT2-page/>) |
| [**JavisDiT: Joint Audio-Video Diffusion Transformer with Hierarchical Spatio-Temporal Prior Synchronization**](<https://arxiv.org/abs/2503.23377>) | 2026 | ICLR | [Code](<https://github.com/JavisVerse/JavisDiT>) · [Project](<https://javisverse.github.io/JavisDiT-page/>) · [Data](<https://huggingface.co/datasets/JavisVerse/JavisBench>) |
| [**JoVA: Unified Multimodal Learning for Joint Video-Audio Generation and Editing**](<https://arxiv.org/abs/2512.13677>) | 2026 | ECCV | [Code](<https://github.com/Visual-AI/JoVA>) · [Project](<https://visual-ai.github.io/jova/>) |
| [**LTX-2.3**](<https://huggingface.co/Lightricks/LTX-2.3>) | 2026 | — | [Code](<https://github.com/Lightricks/LTX-2>) |
| [**LTX-2.5**](<https://huggingface.co/Lightricks/LTX-2.5>) | 2026 | — | — |
| [**LTX-2: Efficient Joint Audio-Visual Foundation Model**](<https://arxiv.org/abs/2601.03233>) | 2026 | arXiv | [Code](<https://github.com/Lightricks/LTX-2>) · [Project](<https://ltx.io/>) · [Demo](<https://app.ltx.studio/ltx-2-playground/i2v>) |
| [**MiniMax-H3: Open Omni-Modal Video-Audio Generation**](<https://www.minimax.io/blog/minimax-h3>) | 2026 | — | [Code](<https://github.com/MiniMax-AI/MiniMax-H3>) · [Models](<https://huggingface.co/MiniMaxAI/MiniMax-H3>) |
| [**Omni-LiveAvatar: Minute-Level Real-Time Streaming Joint Audio-Video Avatar Generation**](<https://arxiv.org/abs/2608.13602>) | 2026 | arXiv | [GitHub](<https://github.com/Aoko955/Omni-LiveAvatar>) · [Project](<https://aoko955.github.io/Omni-LiveAvatar/>) |
| [**Speed by Simplicity: A Single-Stream Architecture for Fast Audio-Video Generative Foundation Model**](<https://arxiv.org/abs/2603.21986>) | 2026 | arXiv | [Code](<https://github.com/GAIR-NLP/daVinci-MagiHuman>) · [Demo](<https://huggingface.co/spaces/SII-GAIR/daVinci-MagiHuman>) |
| [**TaoMate-HD: Progressive-Resolution Autoregressive Audio-Video Generation**](<https://arxiv.org/abs/2611.03394>) | 2026 | arXiv | [Code](<https://github.com/TaoLiveAIGC/TaoMate-HD>) · [Project](<https://taoliveaigc.github.io/TaoMate-HD>) |
| [**TaoMate: Anchor-Guided Memory Bridging Evolving and Reference States for Real-Time Audio-Video Digital Human Generation**](<https://arxiv.org/abs/2607.24359>) | 2026 | arXiv | [Code](<https://github.com/TaoLiveAIGC/TaoMate>) · [Project](<https://taoliveaigc.github.io/TaoMate>) |
| [**UniAVC: Unified Audio-Video Creation via Progressive Training and Asymmetric Scheduling**](<https://arxiv.org/abs/2610.24791>) | 2026 | arXiv | [Code](<https://github.com/HKUST-LongGroup/UniAVC>) · [Project](<https://hkust-longgroup.github.io/UniAVC>) |
| [**UniAVGen: Unified Audio and Video Generation with Asymmetric Cross-Modal Interactions**](<https://arxiv.org/abs/2511.03334>) | 2026 | CVPR | [Code](<https://github.com/mcg-nju/sora2-mini>) · [Project](<https://mcg-nju.github.io/UniAVGen/>) |
| [**Video = World + Event Stream**](<https://arxiv.org/abs/2607.15038>) | 2026 | arXiv | [Project](<https://wan-streamer.com/v0.3/>) |
| [**Wan-Streamer v0.1: End-to-end Real-time Interactive Foundation Models**](<https://arxiv.org/abs/2606.25041>) | 2026 | arXiv | [Project](<https://wan-streamer.com/>) |
| [**Wan-Streamer v0.2: Higher Resolution, Same Latency**](<https://arxiv.org/abs/2607.04443>) | 2026 | arXiv | [Project](<https://wan-streamer.com/>) |
| [**$^R$FLAV: Rolling Flow matching for infinite Audio Video generation**](<https://arxiv.org/abs/2503.08307>) | 2025 | arXiv | [Code](<https://github.com/ErgastiAlex/R-FLAV>) |
| [**A Simple but Strong Baseline for Sounding Video Generation: Effective Adaptation of Audio and Video Diffusion Models for Joint Generation**](<https://arxiv.org/abs/2409.17550>) | 2025 | arXiv | [Code](<https://github.com/sonyresearch/svg_baseline>) |
| [**AV-DiT: Taming Image Diffusion Transformers for Efficient Joint Audio and Video Generation**](<https://doi.org/10.1145/3746027.3755713>) | 2025 | ACM MM | — |
| [**Kling AI Launches Video 2.6 Model with Simultaneous Audio-Visual Generation Capability**](<https://ir.kuaishou.com/news-releases/news-release-details/kling-ai-launches-video-26-model-simultaneous-audio-visual/>) | 2025 | — | — |
| [**Ovi: Twin Backbone Cross-Modal Fusion for Audio-Video Generation**](<https://arxiv.org/abs/2510.01284>) | 2025 | arXiv | [Code](<https://github.com/character-ai/Ovi>) · [Project](<https://aaxwaz.github.io/Ovi>) |
| [**PixVerse v5.5: Smarter Video Generation, Better Results**](<https://www.eachlabs.ai/blog/pixverse-v5-5-smarter-video-generation-better-results>) | 2025 | — | [Demo](<https://app.pixverse.ai/>) |
| [**Seedance 1.5 pro: A Native Audio-Visual Joint Generation Foundation Model**](<https://arxiv.org/abs/2512.13507>) | 2025 | arXiv | [Project](<https://seed.bytedance.com/seedance1_5_pro>) |
| [**Sora 2 System Card**](<https://openai.com/index/sora-2-system-card/>) | 2025 | — | [Project](<https://openai.com/index/sora-2/>) |
| [**UniVerse-1: Unified Audio-Video Generation via Stitching of Experts**](<https://arxiv.org/abs/2509.06155>) | 2025 | arXiv | [Code](<https://github.com/Dorniwang/UniVerse-1-code>) · [Project](<https://dorniwang.github.io/UniVerse-1/>) |
| [**Veo 3.1: Video Generation with Native Audio**](<https://deepmind.google/models/veo/>) | 2025 | — | — |
| [**AV-Link: Temporally-Aligned Diffusion Features for Cross-Modal Audio-Video Generation**](<https://arxiv.org/abs/2412.15191>) | 2024 | arXiv | [Code](<https://github.com/snap-research/AVLink>) · [Project](<https://snap-research.github.io/AVLink/>) |
| [**CoDi-2: In-Context, Interleaved, and Interactive Any-to-Any Generation**](<https://arxiv.org/abs/2311.18775>) | 2024 | arXiv | — |
| [**Movie Gen: A Cast of Media Foundation Models**](<https://arxiv.org/abs/2410.13720>) | 2024 | arXiv | [Code](<https://github.com/facebookresearch/MovieGenBench>) |
| [**Any-to-Any Generation via Composable Diffusion**](<https://arxiv.org/abs/2305.11846>) | 2023 | NeurIPS | [Code](<https://github.com/microsoft/i-Code/tree/main/i-Code-V3>) · [Project](<https://codi-gen.github.io/>) |
| [**MM-Diffusion: Learning Multi-Modal Diffusion Models for Joint Audio and Video Generation**](<https://arxiv.org/abs/2212.09478>) | 2023 | CVPR | [Code](<https://github.com/researchmm/mm-diffusion>) |

### Audio-Video Understanding

#### Task-Specific Models

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Question-Aware Gaussian Experts for Audio-Visual Question Answering**](<https://openaccess.thecvf.com/content/CVPR2025/html/Kim_Question-Aware_Gaussian_Experts_for_Audio-Visual_Question_Answering_CVPR_2025_paper.html>) | 2025 | CVPR | [Code](<https://github.com/AIM-SKKU/QA-TIGER>) · [Project](<https://aim-skku.github.io/QA-TIGER/>) |
| [**Towards Audio-Visual Navigation in Noisy Environments: A Large-Scale Benchmark Dataset and an Architecture Considering Multiple Sound-Sources**](<https://doi.org/10.1609/aaai.v39i14.33608>) | 2025 | AAAI | — |
| [**AVSegFormer: Audio-Visual Segmentation with Transformer**](<https://arxiv.org/abs/2307.01146>) | 2024 | AAAI | — |
| [**Benchmarking Audio Visual Segmentation for Long-Untrimmed Videos**](<https://doi.org/10.1109/cvpr52733.2024.02143>) | 2024 | CVPR | — |
| [**Audio Visual Language Maps for Robot Navigation**](<https://arxiv.org/abs/2303.07522>) | 2023 | Proceedings of the International Symposium on Experimental Robotics (ISER) | [Code](<https://github.com/avlmaps/AVLMaps>) · [Project](<https://avlmaps.github.io/>) |
| [**A Closer Look at Weakly-Supervised Audio-Visual Source Localization**](<https://doi.org/10.52202/068431-2720>) | 2022 | NeurIPS | [Code](<https://github.com/stoneMo/SLAVC>) |
| [**Attention Bottlenecks for Multimodal Fusion**](<https://arxiv.org/abs/2107.00135>) | 2021 | NeurIPS | [Code](<https://github.com/google-research/scenic/tree/main/scenic/projects/mbt>) |
| [**Cross-Attentional Audio-Visual Fusion for Weakly-Supervised Action Localization**](<https://openreview.net/forum?id=hWr3e3r-oH5>) | 2021 | ICLR | — |
| [**Learning to Set Waypoints for Audio-Visual Navigation**](<https://arxiv.org/abs/2008.09622>) | 2021 | ICLR | [Code](<https://github.com/facebookresearch/sound-spaces>) · [Project](<https://vision.cs.utexas.edu/projects/audio_visual_waypoints/>) |
| [**Localizing Visual Sounds the Hard Way**](<https://doi.org/10.1109/CVPR46437.2021.01659>) | 2021 | CVPR | [Code](<https://github.com/hche11/Localizing-Visual-Sounds-the-Hard-Way>) |
| [**Soundspaces: Audio-visual navigation in 3d environments**](<https://doi.org/10.1007/978-3-030-58539-6_2>) | 2020 | ECCV | [Code](<https://github.com/facebookresearch/sound-spaces>) |
| [**Unified Multisensory Perception: Weakly-Supervised Audio-Visual Video Parsing**](<https://doi.org/10.1007/978-3-030-58580-8_26>) | 2020 | ECCV | [Code](<https://github.com/YapengTian/AVVP-ECCV20>) |
| [**EPIC-Fusion: Audio-Visual Temporal Binding for Egocentric Action Recognition**](<https://doi.org/10.1109/ICCV.2019.00559>) | 2019 | ICCV | [Code](<https://github.com/ekazakos/temporal-binding-network>) |
| [**The Sound of Motions**](<https://arxiv.org/abs/1904.05979>) | 2019 | ICCV | [Code](<https://github.com/hangzhaomit/Sound-of-Motions>) |
| [**Audio-Visual Event Localization in Unconstrained Videos**](<https://doi.org/10.1007/978-3-030-01216-8_16>) | 2018 | ECCV | [Code](<https://github.com/YapengTian/AVE-ECCV18>) |
| [**Objects that Sound**](<https://arxiv.org/abs/1712.06651>) | 2018 | ECCV | — |
| [**The Sound of Pixels**](<https://arxiv.org/abs/1804.03160>) | 2018 | ECCV | [Code](<https://github.com/hangzhaomit/Sound-of-Pixels>) |

#### Self-Supervised Learning

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Pushing the Frontier of Audiovisual Perception with Large-Scale Multimodal Correspondence Learning**](<https://openaccess.thecvf.com/content/CVPR2026/html/Vyas_Pushing_the_Frontier_of_Audiovisual_Perception_with_Large-Scale_Multimodal_Correspondence_CVPR_2026_paper.html>) | 2026 | CVPR | [Code](<https://github.com/facebookresearch/perception_models>) · [Project](<https://ai.meta.com/research/publications/pushing-the-frontier-of-audiovisual-perception-with-large-scale-multimodal-correspondence-learning/>) · [Models](<https://huggingface.co/facebook/pe-a-frame-base>) |
| [**Cav-mae sync: Improving contrastive audio-visual mask autoencoders via fine-grained alignment**](<https://openaccess.thecvf.com/content/CVPR2025/html/Araujo_CAV-MAE_Sync_Improving_Contrastive_Audio-Visual_Mask_Autoencoders_via_Fine-Grained_Alignment_CVPR_2025_paper.html>) | 2025 | CVPR | — |
| [**InternVideo2: Scaling Foundation Models for Multimodal Video Understanding**](<https://arxiv.org/abs/2403.15377>) | 2024 | ECCV | [Code](<https://github.com/OpenGVLab/InternVideo/tree/main/InternVideo2/>) |
| [**LanguageBind: Extending Video-Language Pretraining to N-modality by Language-based Semantic Alignment**](<https://arxiv.org/abs/2310.01852>) | 2024 | ICLR | [Code](<https://github.com/PKU-YuanGroup/LanguageBind>) |
| [**Contrastive Audio-Visual Masked Autoencoder**](<https://arxiv.org/abs/2210.07839>) | 2023 | ICLR | — |
| [**ImageBind: One Embedding Space To Bind Them All**](<https://doi.org/10.1109/cvpr52729.2023.01457>) | 2023 | CVPR | [Code](<https://github.com/facebookresearch/ImageBind>) |
| [**Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation**](<https://doi.org/10.1109/icassp49357.2023.10095969>) | 2023 | ICASSP | [Code](<https://github.com/laion-ai/clap>) |
| [**ONE-PEACE: Exploring One General Representation Model Toward Unlimited Modalities**](<https://arxiv.org/abs/2305.11172>) | 2023 | arXiv | [Code](<https://github.com/OFA-Sys/ONE-PEACE>) |
| [**VALOR: Vision-Audio-Language Omni-Perception Pretraining Model and Dataset**](<https://arxiv.org/abs/2304.08345>) | 2023 | arXiv | [Code](<https://github.com/TXH-mercury/VALOR>) |
| [**AudioCLIP: Extending CLIP to Image, Text and Audio**](<https://doi.org/10.1109/ICASSP43922.2022.9747631>) | 2022 | ICASSP | [Code](<https://github.com/AndreyGuzhov/AudioCLIP>) |
| [**Masked Autoencoders that Listen**](<https://arxiv.org/abs/2207.06405>) | 2022 | NeurIPS | [Code](<https://github.com/facebookresearch/AudioMAE>) |
| [**Learning Transferable Visual Models From Natural Language Supervision**](<https://arxiv.org/abs/2103.00020>) | 2021 | ICML | [Code](<https://github.com/openai/CLIP>) |

#### MLLM Generalists

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**video-SALMONN S: Memory-Enhanced Streaming Audio-Visual LLM**](<https://proceedings.mlr.press/v306/sun26s.html>) | 2026 | ICML | — |
| [**Aligned Better, Listen Better for Audio-Visual Large Language Models**](<https://arxiv.org/abs/2504.02061>) | 2025 | ICLR | — |
| [**AVicuna: Audio-Visual LLM with Interleaver and Context-Boundary Alignment for Temporal Referential Dialogue**](<https://arxiv.org/abs/2403.16276>) | 2025 | AAAI | — |
| [**Crab: A Unified Audio-Visual Scene Understanding Model with Explicit Cooperation**](<https://arxiv.org/abs/2503.13068>) | 2025 | arXiv | — |
| [**LongVALE: Vision-Audio-Language-Event Benchmark Towards Time-Aware Omni-Modal Perception of Long Videos**](<https://openaccess.thecvf.com/content/CVPR2025/html/Geng_LongVALE_Vision-Audio-Language-Event_Benchmark_Towards_Time-Aware_Omni-Modal_Perception_of_Long_Videos_CVPR_2025_paper.html>) | 2025 | CVPR | [Code](<https://github.com/ttgeng233/longvale>) · [Project](<https://ttgeng233.github.io/LongVALE/>) |
| [**OmniVinci: Enhancing Architecture and Data for Omni-Modal Understanding LLM**](<https://arxiv.org/abs/2510.15870>) | 2025 | arXiv | [Code](<https://github.com/NVlabs/OmniVinci>) · [Project](<https://nvlabs.github.io/OmniVinci/>) |
| [**CREMA: Generalizable and Efficient Video-Language Reasoning via Multimodal Modular Fusion**](<https://arxiv.org/abs/2402.05889>) | 2024 | arXiv | [Code](<https://github.com/Yui010206/CREMA>) |
| [**Emotion-LLaMA: Multimodal Emotion Recognition and Reasoning with Instruction Tuning**](<https://doi.org/10.52202/079017-3518>) | 2024 | NeurIPS | — |
| [**Listen, Think, and Understand**](<https://openreview.net/forum?id=nBZBPXdJlC>) | 2024 | ICLR | [Code](<https://github.com/YuanGongND/ltu>) · [Demo](<https://huggingface.co/spaces/yuangongfdu/ltu>) |
| [**Meerkat: Audio-Visual Large Language Model for Grounding in Space and Time**](<https://doi.org/10.1007/978-3-031-73039-9_4>) | 2024 | ECCV | — |
| [**Megrez-3B-Omni: Efficient Omni-Modal Foundation Model**](<https://github.com/infinigence/Infini-Megrez-Omni>) | 2024 | — | — |
| [**MultiPLY: A Multisensory Object-Centric Embodied Large Language Model in 3D World**](<https://arxiv.org/abs/2401.08577>) | 2024 | CVPR | [Project](<https://vis-www.cs.umass.edu/MultiPLY/>) |
| [**OMCAT: Omni Context Aware Transformer**](<https://arxiv.org/abs/2410.12109>) | 2024 | arXiv | [Project](<https://om-cat.github.io>) |
| [**OneLLM: One Framework to Align All Modalities with Language**](<https://arxiv.org/abs/2312.03700>) | 2024 | CVPR | [Code](<https://github.com/csuhan/OneLLM>) |
| [**SALMONN: Towards Generic Hearing Abilities for Large Language Models**](<https://arxiv.org/abs/2310.13289>) | 2024 | ICLR | [Code](<https://github.com/bytedance/salmonn>) · [Demo](<https://huggingface.co/spaces/tsinghua-ee/SALMONN-7B-gradio>) |
| [**Uni-MoE: Scaling Unified Multimodal LLMs with Mixture of Experts**](<https://arxiv.org/abs/2405.11273>) | 2024 | arXiv | [Code](<https://github.com/HITsz-TMG/UMOE-Scaling-Unified-Multimodal-LLMs>) |
| [**video-SALMONN: Speech-Enhanced Audio-Visual Large Language Models**](<https://proceedings.mlr.press/v235/sun24l.html>) | 2024 | ICML | — |
| [**VideoLLaMA 2: Advancing Spatial-Temporal Modeling and Audio Understanding in Video-LLMs**](<https://arxiv.org/abs/2406.07476>) | 2024 | arXiv | [Code](<https://github.com/DAMO-NLP-SG/VideoLLaMA2/tree/audio_visual>) |
| [**X-InstructBLIP: A Framework for Aligning X-Modal Instruction-Aware Representations to LLMs and Emergent Cross-Modal Reasoning**](<https://openreview.net/forum?id=OvoRkDRLVr>) | 2024 | ECCV | [Code](<https://github.com/artemisp/lavis-xinstructblip>) |
| [**AnyMAL: An Efficient and Scalable Any-Modality Augmented Language Model**](<https://arxiv.org/abs/2309.16058>) | 2023 | arXiv | — |
| [**Audio-Visual LLM for Video Understanding**](<https://arxiv.org/abs/2312.06720>) | 2023 | arXiv | — |
| [**BuboGPT: Enabling Visual Grounding in Multi-Modal LLMs**](<https://arxiv.org/abs/2307.08581>) | 2023 | arXiv | [Code](<https://github.com/magic-research/bubogpt>) |
| [**ChatBridge: Bridging Modalities with Large Language Model as a Language Catalyst**](<https://arxiv.org/abs/2305.16103>) | 2023 | arXiv | [Code](<https://github.com/joez17/chatbridge>) |
| [**eP-ALM: Efficient Perceptual Augmentation of Language Models**](<https://arxiv.org/abs/2303.11403>) | 2023 | ICCV | [Code](<https://github.com/mshukor/eP-ALM>) · [Project](<https://mshukor.github.io/eP-ALM.github.io/>) |
| [**ImageBind-LLM: Multi-modality Instruction Tuning**](<https://arxiv.org/abs/2309.03905>) | 2023 | arXiv | [Code](<https://github.com/opengvlab/llama-adapter>) |
| [**LLaSM: Large Language and Speech Model**](<https://arxiv.org/abs/2308.15930>) | 2023 | arXiv | [Code](<https://github.com/linksoul-ai/llasm>) |
| [**Macaw-LLM: Multi-Modal Language Modeling with Image, Audio, Video, and Text Integration**](<https://arxiv.org/abs/2306.09093>) | 2023 | arXiv | [Code](<https://github.com/lyuchenyang/macaw-llm>) |
| [**Music Understanding LLaMA: Advancing Text-to-Music Generation with Question Answering and Captioning**](<https://arxiv.org/abs/2308.11276>) | 2023 | arXiv | [Code](<https://github.com/crypto-code/mu-llama>) |
| [**PandaGPT: One Model to Instruction-Follow Them All**](<https://arxiv.org/abs/2305.16355>) | 2023 | arXiv | [Code](<https://github.com/yxuansu/pandagpt>) · [Project](<https://panda-gpt.github.io/>) |
| [**Pengi: An Audio Language Model for Audio Tasks**](<https://arxiv.org/abs/2305.11834>) | 2023 | arXiv | [Code](<https://github.com/microsoft/Pengi>) |
| [**Qwen-Audio: Advancing Universal Audio Understanding via Unified Large-Scale Audio-Language Models**](<https://arxiv.org/abs/2311.07919>) | 2023 | arXiv | [Code](<https://github.com/QwenLM/Qwen-Audio>) |
| [**Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding**](<https://doi.org/10.18653/v1/2023.emnlp-demo.49>) | 2023 | EMNLP Demo | [Code](<https://github.com/damo-nlp-sg/video-llama>) · [Demo](<https://huggingface.co/spaces/DAMO-NLP-SG/Video-LLaMA>) |
| [**X-LLM: Bootstrapping Advanced Large Language Models by Treating Multi-Modalities as Foreign Languages**](<https://arxiv.org/abs/2305.04160>) | 2023 | arXiv | [Code](<https://github.com/phellonchen/x-llm>) · [Project](<https://x-llm.github.io>) |

### Unified Architectures

#### Fully Autoregressive

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**EMOVA: Empowering Language Models to See, Hear and Speak with Vivid Emotions**](<https://openaccess.thecvf.com/content/CVPR2025/html/Chen_EMOVA_Empowering_Language_Models_to_See_Hear_and_Speak_with_CVPR_2025_paper.html>) | 2025 | CVPR | [Project](<https://emova-ollm.github.io/>) |
| [**Harmonizing Visual Representations for Unified Multimodal Understanding and Generation**](<https://arxiv.org/abs/2503.21979>) | 2025 | arXiv | [Code](<https://github.com/wusize/Harmon>) |
| [**MIO: A Foundation Model on Multimodal Tokens**](<https://doi.org/10.18653/v1/2025.emnlp-main.255>) | 2025 | EMNLP | [Code](<https://github.com/mio-team/mio>) |
| [**Transfer between Modalities with MetaQueries**](<https://arxiv.org/abs/2504.06256>) | 2025 | arXiv | [Project](<https://xichenpan.com/metaquery>) |
| [**ANOLE: An Open, Autoregressive, Native Large Multimodal Models for Interleaved Image-Text Generation**](<https://arxiv.org/abs/2407.06135>) | 2024 | arXiv | [Code](<https://github.com/gair-nlp/anole>) · [Demo](<https://huggingface.co/spaces/ethanchern/Anole>) |
| [**AnyGPT: Unified Multimodal LLM with Discrete Sequence Modeling**](<https://arxiv.org/abs/2402.12226>) | 2024 | arXiv | [Code](<https://github.com/OpenMOSS/AnyGPT>) · [Project](<https://junzhan2000.github.io/AnyGPT.github.io/>) |
| [**Chameleon: Mixed-Modal Early-Fusion Foundation Models**](<https://arxiv.org/abs/2405.09818>) | 2024 | arXiv | [Code](<https://github.com/facebookresearch/chameleon>) |
| [**Emu3: Next-Token Prediction is All You Need**](<https://arxiv.org/abs/2409.18869>) | 2024 | arXiv | [Code](<https://github.com/baaivision/emu3>) |
| [**ILLUME: Illuminating Your LLMs to See, Draw, and Self-Enhance**](<https://arxiv.org/abs/2412.06673>) | 2024 | arXiv | — |
| [**Liquid: Language Models are Scalable and Unified Multi-modal Generators**](<https://arxiv.org/abs/2412.04332>) | 2024 | arXiv | [Code](<https://github.com/FoundationVision/Liquid>) · [Project](<https://foundationvision.github.io/Liquid/>) |
| [**SynerGen-VL: Towards Synergistic Image Understanding and Generation with Vision Experts and Token Folding**](<https://arxiv.org/abs/2412.09604>) | 2024 | arXiv | — |
| [**Unified-IO 2: Scaling Autoregressive Multimodal Models with Vision, Language, Audio, and Action**](<https://arxiv.org/abs/2312.17172>) | 2024 | CVPR | [Code](<https://github.com/allenai/unified-io-2>) · [Project](<https://unified-io-2.allenai.org/>) |
| [**World model on million-length video and language with blockwise ringattention**](<https://arxiv.org/abs/2402.08268>) | 2024 | arXiv | [Code](<https://github.com/LargeWorldModel/LWM>) |

#### Fully Diffusion

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**FUDOKI: Discrete Flow-based Unified Understanding and Generation via Kinetic-Optimal Velocities**](<https://arxiv.org/abs/2505.20147>) | 2025 | arXiv | — |
| [**MMaDA: Multimodal Large Diffusion Language Models**](<https://arxiv.org/abs/2505.15809>) | 2025 | NeurIPS | [Code](<https://github.com/Gen-Verse/MMaDA>) · [Demo](<https://huggingface.co/spaces/Gen-Verse/MMaDA>) |
| [**Muddit: Liberating Generation Beyond Text-to-Image with a Unified Discrete Diffusion Model**](<https://arxiv.org/abs/2505.23606>) | 2025 | arXiv | [Code](<https://github.com/M-E-AGI-Lab/Muddit>) |
| [**Unified Multimodal Discrete Diffusion**](<https://arxiv.org/abs/2503.20853>) | 2025 | arXiv | — |
| [**Dual Diffusion for Unified Image Generation and Understanding**](<https://arxiv.org/abs/2501.00289>) | 2024 | arXiv | [Code](<https://github.com/zijieli-Jlee/Dual-Diffusion>) · [Project](<https://zijieli-jlee.github.io/dualdiff.github.io/>) |

#### Decoupled Hybrid

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Cosmos 3: Omnimodal World Models for Physical AI**](<https://arxiv.org/abs/2606.02800>) | 2026 | arXiv | [Code](<https://github.com/NVIDIA/cosmos>) · [Project](<https://research.nvidia.com/labs/cosmos-lab/cosmos3/index.html>) · [Models](<https://huggingface.co/collections/nvidia/cosmos3>) |
| [**MAViD: A Multimodal Framework for Audio-Visual Dialogue Understanding and Generation**](<https://arxiv.org/abs/2512.03034>) | 2026 | SIGGRAPH | [Project](<https://carlyx.github.io/MAViD/>) |
| [**Baichuan-Omni-1.5 Technical Report**](<https://arxiv.org/abs/2501.15368>) | 2025 | arXiv | [Code](<https://github.com/baichuan-inc/baichuan-omni-1.5>) |
| [**BLIP3-o: A Family of Fully Open Unified Multimodal Models -- Architecture, Training and Dataset**](<https://arxiv.org/abs/2505.09568>) | 2025 | arXiv | [Code](<https://github.com/BLIP3o/BLIP3o>) |
| [**Emerging Properties in Unified Multimodal Pretraining**](<https://arxiv.org/abs/2505.14683>) | 2025 | arXiv | [Code](<https://github.com/ByteDance-Seed/Bagel>) · [Project](<https://bagel-ai.org/>) |
| [**EMMA: Efficient Multimodal Understanding, Generation, and Editing with a Unified Architecture**](<https://arxiv.org/abs/2512.04810>) | 2025 | arXiv | — |
| [**Janus-Pro: Unified Multimodal Understanding and Generation with Data and Model Scaling**](<https://arxiv.org/abs/2501.17811>) | 2025 | arXiv | [Code](<https://github.com/deepseek-ai/janus>) |
| [**JanusFlow: Harmonizing Autoregression and Rectified Flow for Unified Multimodal Understanding and Generation**](<https://doi.org/10.1109/CVPR52734.2025.00725>) | 2025 | CVPR | [Code](<https://github.com/deepseek-ai/Janus>) |
| [**JavisGPT: A Unified Multi-modal LLM for Sounding-Video Comprehension and Generation**](<https://arxiv.org/abs/2512.22905>) | 2025 | NeurIPS | [Code](<https://github.com/JavisVerse/JavisGPT>) |
| [**M2-Omni: Advancing Omni-MLLM for Comprehensive Modality Support with Competitive Performance**](<https://arxiv.org/abs/2502.18778>) | 2025 | arXiv | — |
| [**Ming-Omni: A Unified Multimodal Model for Perception and Generation**](<https://arxiv.org/abs/2506.09344>) | 2025 | arXiv | [Code](<https://github.com/inclusionAI/Ming>) · [Project](<https://lucaria-academy.github.io/Ming-Omni>) |
| [**MiniCPM-o 2.6: A GPT-4o Level MLLM for Vision, Speech and Multimodal Live Streaming on Your Phone**](<https://huggingface.co/openbmb/MiniCPM-o-2_6>) | 2025 | — | [Code](<https://github.com/OpenBMB/MiniCPM-o>) |
| [**MMAR: Towards Lossless Multi-Modal Auto-Regressive Probabilistic Modeling**](<https://doi.org/10.1109/CVPR52734.2025.00747>) | 2025 | CVPR | — |
| [**OmniMamba: Efficient and Unified Multimodal Understanding and Generation via State Space Models**](<https://arxiv.org/abs/2503.08686>) | 2025 | arXiv | [Code](<https://github.com/hustvl/omnimamba>) |
| [**Qwen2.5-Omni Technical Report**](<https://arxiv.org/abs/2503.20215>) | 2025 | arXiv | [Code](<https://github.com/QwenLM/Qwen2.5-Omni>) · [Project](<https://qwenlm.github.io/blog/qwen2.5-omni/>) |
| [**Qwen3-Omni Technical Report**](<https://arxiv.org/abs/2509.17765>) | 2025 | arXiv | [Code](<https://github.com/QwenLM/Qwen3-Omni>) |
| [**Show-o2: Improved Native Unified Multimodal Models**](<https://arxiv.org/abs/2506.15564>) | 2025 | arXiv | [Code](<https://github.com/showlab/Show-o>) · [Demo](<https://huggingface.co/spaces/showlab/Show-o>) |
| [**Show-o: One Single Transformer to Unify Multimodal Understanding and Generation**](<https://arxiv.org/abs/2408.12528>) | 2025 | ICLR | [Code](<https://github.com/showlab/Show-o>) |
| [**Unified Autoregressive Visual Generation and Understanding with Continuous Tokens**](<https://arxiv.org/abs/2503.13436>) | 2025 | arXiv | — |
| [**VARGPT: Unified Understanding and Generation in a Visual Autoregressive Multimodal Large Language Model**](<https://arxiv.org/abs/2501.12327>) | 2025 | arXiv | [Code](<https://github.com/VARGPT-family/VARGPT>) · [Project](<https://vargpt-1.github.io/>) · [Data](<https://huggingface.co/datasets/VARGPT-family/VARGPT_datasets>) · [Models](<https://huggingface.co/VARGPT-family/VARGPT_LLaVA-v1>) |
| [**VILA-U: A Unified Foundation Model Integrating Visual Understanding and Generation**](<https://arxiv.org/abs/2409.04429>) | 2025 | ICLR | [Code](<https://github.com/mit-han-lab/vila-u>) |
| [**VITA-1.5: Towards GPT-4o Level Real-Time Vision and Speech Interaction**](<https://openreview.net/forum?id=8PUzLga3lU>) | 2025 | NeurIPS | [Code](<https://github.com/VITA-MLLM/VITA>) · [Demo](<https://huggingface.co/spaces/VITA-MLLM/VITA-1.5>) |
| [**Emu: Generative Pretraining in Multimodality**](<https://openreview.net/forum?id=mL8Q9OOamV>) | 2024 | ICLR | — |
| [**Janus: Decoupling Visual Encoding for Unified Multimodal Understanding and Generation**](<https://arxiv.org/abs/2410.13848>) | 2024 | arXiv | [Code](<https://github.com/deepseek-ai/Janus>) |
| [**LMFusion: Adapting Pretrained Language Models for Multimodal Generation**](<https://arxiv.org/abs/2412.15188>) | 2024 | arXiv | — |
| [**Lyra: An Efficient and Speech-Centric Framework for Omni-Cognition**](<https://arxiv.org/abs/2412.09501>) | 2024 | arXiv | [Code](<https://github.com/dvlab-research/Lyra>) |
| [**Mini-Omni2: Towards Open-source GPT-4o with Vision, Speech and Duplex Capabilities**](<https://arxiv.org/abs/2410.11190>) | 2024 | arXiv | [Code](<https://github.com/gpt-omni/mini-omni2>) |
| [**MonoFormer: One Transformer for Both Diffusion and Autoregression**](<https://arxiv.org/abs/2409.16280>) | 2024 | arXiv | [Code](<https://github.com/monoformer/monoformer>) · [Project](<https://monoformer.github.io/>) |
| [**MUSE-VL: Modeling Unified VLM through Semantic Discrete Encoding**](<https://arxiv.org/abs/2411.17762>) | 2024 | arXiv | — |
| [**SEED-X: Multimodal Models with Unified Multi-Granularity Comprehension and Generation**](<https://arxiv.org/abs/2404.14396>) | 2024 | arXiv | [Code](<https://github.com/ailab-cvc/seed-x>) |
| [**Tokenflow: Unified Image Tokenizer for Multimodal Understanding and Generation**](<https://arxiv.org/abs/2412.03069>) | 2024 | arXiv | [Code](<https://github.com/ByteFlow-AI/TokenFlow>) · [Project](<https://byteflow-ai.github.io/TokenFlow/>) |
| [**Transfusion: Predict the Next Token and Diffuse Images with One Multi-Modal Model**](<https://arxiv.org/abs/2408.11039>) | 2024 | arXiv | — |
| [**Video-LaVIT: Unified Video-Language Pre-training with Decoupled Visual-Motional Tokenization**](<https://arxiv.org/abs/2402.03161>) | 2024 | arXiv | [Code](<https://github.com/jy0205/lavit>) |
| [**DreamLLM: Synergistic Multimodal Comprehension and Creation**](<https://arxiv.org/abs/2309.11499>) | 2023 | arXiv | [Code](<https://github.com/RunpeiDong/DreamLLM>) · [Project](<https://dreamllm.github.io>) |
| [**Making LLaMA See and Draw with SEED Tokenizer**](<https://arxiv.org/abs/2310.01218>) | 2023 | arXiv | [Code](<https://github.com/AILab-CVC/SEED>) |
| [**Planting a Seed of Vision in Large Language Model**](<https://arxiv.org/abs/2307.08041>) | 2023 | arXiv | [Code](<https://github.com/AILab-CVC/SEED>) · [Demo](<https://huggingface.co/spaces/AILab-CVC/SEED-LLaMA>) |
| [**Unified Language-Vision Pretraining in LLM with Dynamic Discrete Visual Tokenization**](<https://arxiv.org/abs/2309.04669>) | 2023 | arXiv | [Code](<https://github.com/jy0205/LaVIT>) |

#### Modular / Agentic

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Efficient Generative Multimodal Integration (EGMI): Enabling Audio Generation from Text-Image Pairs through Alignment with Large Language Models**](<https://openreview.net/pdf/462424e66f7fea533a443a35104ca1dae8e95518.pdf>) | 2024 | — | — |
| [**EmpathyEar: An Open-source Avatar Multimodal Empathetic Chatbot**](<https://arxiv.org/abs/2406.15177>) | 2024 | arXiv | — |
| [**ModaVerse: Efficiently Transforming Modalities with LLMs**](<https://doi.org/10.1109/cvpr52733.2024.02512>) | 2024 | CVPR | [Code](<https://github.com/xinke-wang/ModaVerse>) |
| [**NExT-GPT: Any-to-Any Multimodal LLM**](<https://arxiv.org/abs/2309.05519>) | 2024 | ICML | — |
| [**Spider: Any-to-Many Multimodal LLM**](<https://arxiv.org/abs/2411.09439>) | 2024 | arXiv | [Code](<https://github.com/Layjins/Spider>) |
| [**Towards Multi-Modal Mastery: A 4.5B Parameter Truly Multi-Modal Small Language Model**](<https://arxiv.org/abs/2411.05903>) | 2024 | arXiv | — |
| [**UnifiedMLLM: Enabling Unified Representation for Multi-modal Multi-tasks With Large Language Model**](<https://arxiv.org/abs/2408.02503>) | 2024 | arXiv | [Code](<https://github.com/lzw-lzw/unifiedmllm>) |
| [**VITA: Towards Open-Source Interactive Omni Multimodal LLM**](<https://arxiv.org/abs/2408.05211>) | 2024 | arXiv | [Code](<https://github.com/vita-mllm/vita>) · [Project](<https://vita-home.github.io>) |
| [**X-VILA: Cross-Modality Alignment for Large Language Model**](<https://arxiv.org/abs/2405.19335>) | 2024 | arXiv | — |
| [**AudioGPT: Understanding and Generating Speech, Music, Sound, and Talking Head**](<https://arxiv.org/abs/2304.12995>) | 2023 | arXiv | [Code](<https://github.com/AIGC-Audio/AudioGPT>) |
| [**HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in HuggingFace**](<https://arxiv.org/abs/2303.17580>) | 2023 | NeurIPS | [Code](<https://github.com/microsoft/JARVIS>) · [Demo](<https://huggingface.co/spaces/microsoft/HuggingGPT>) |
| [**MusicAgent: An AI Agent for Music Understanding and Generation with Large Language Models**](<https://arxiv.org/abs/2310.11954>) | 2023 | arXiv | [Code](<https://github.com/microsoft/muzic>) |
| [**Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models**](<https://arxiv.org/abs/2303.04671>) | 2023 | arXiv | [Code](<https://github.com/microsoft/visual-chatgpt>) |

### Audio-Video Tokenization

#### Audio Tokenizers

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Language-Codec: Bridging Discrete Codec Representations and Speech Language Models**](<https://doi.org/10.18653/v1/2025.acl-long.654>) | 2025 | ACL | [Code](<https://github.com/jishengpeng/languagecodec>) |
| [**Stable Audio Open**](<https://arxiv.org/abs/2407.14358>) | 2025 | ICASSP | [Code](<https://github.com/Stability-AI/stable-audio-tools>) · [Project](<https://stability-ai.github.io/stable-audio-open-demo/>) · [Models](<https://huggingface.co/stabilityai/stable-audio-open-1.0>) |
| [**UniCodec: Unified Audio Codec with Single Domain-Adaptive Codebook**](<https://arxiv.org/abs/2502.20067>) | 2025 | arXiv | — |
| [**Wavtokenizer: an efficient acoustic discrete codec tokenizer for audio language modeling**](<https://arxiv.org/abs/2408.16532>) | 2025 | ICLR | [Code](<https://github.com/jishengpeng/WavTokenizer>) · [Models](<https://huggingface.co/novateur/WavTokenizer-large-speech-75token>) |
| [**AudioLDM 2: Learning Holistic Audio Generation with Self-supervised Pretraining**](<https://doi.org/10.1109/taslp.2024.3399607>) | 2024 | IEEE/ACM Transactions on Audio, Speech, and Language Processing | — |
| [**MERT: Acoustic Music Understanding Model with Large-Scale Self-supervised Training**](<https://arxiv.org/abs/2306.00107>) | 2024 | ICLR | — |
| [**SpeechTokenizer: Unified Speech Tokenizer for Speech Language Models**](<https://arxiv.org/abs/2308.16692>) | 2024 | ICLR | — |
| [**BEATs: Audio Pre-Training with Acoustic Tokenizers**](<https://proceedings.mlr.press/v202/chen23ag.html>) | 2023 | ICML | — |
| [**High-Fidelity Audio Compression with Improved RVQGAN**](<https://arxiv.org/abs/2306.06546>) | 2023 | NeurIPS | [Code](<https://github.com/descriptinc/descript-audio-codec>) |
| [**Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation**](<https://doi.org/10.1109/icassp49357.2023.10095969>) | 2023 | ICASSP | [Code](<https://github.com/laion-ai/clap>) |
| [**Robust Speech Recognition via Large-Scale Weak Supervision**](<https://arxiv.org/abs/2212.04356>) | 2023 | ICML | [Code](<https://github.com/openai/whisper>) |
| [**High Fidelity Neural Audio Compression**](<https://arxiv.org/abs/2210.13438>) | 2022 | arXiv | [Code](<https://github.com/facebookresearch/encodec>) |
| [**Masked Autoencoders that Listen**](<https://arxiv.org/abs/2207.06405>) | 2022 | NeurIPS | [Code](<https://github.com/facebookresearch/AudioMAE>) |
| [**SoundStream: An End-to-End Neural Audio Codec**](<https://doi.org/10.1109/taslp.2021.3129994>) | 2022 | IEEE/ACM Trans. Audio, Speech, Language Process. | — |
| [**AST: Audio Spectrogram Transformer**](<https://doi.org/10.21437/interspeech.2021-698>) | 2021 | Interspeech | [Code](<https://github.com/YuanGongND/ast>) |
| [**HuBERT: Self-Supervised Speech Representation Learning by Masked Prediction of Hidden Units**](<https://openreview.net/forum?id=UKprVqG8N7K>) | 2021 | IEEE/ACM Trans. Audio, Speech, Language Process. | [Code](<https://github.com/facebookresearch/fairseq>) |
| [**w2v-BERT: Combining Contrastive Learning and Masked Language Modeling for Self-Supervised Speech Pre-Training**](<https://arxiv.org/abs/2108.06209>) | 2021 | arXiv | — |

#### Video Tokenizers

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**InfoTok: Adaptive Discrete Video Tokenizer via Information-Theoretic Compression**](<https://openreview.net/forum?id=JEYWpFGzvn>) | 2026 | ICLR | [Code](<https://github.com/YWolfeee/InfoTok>) |
| [**VideoFlexTok: Flexible-Length Coarse-to-Fine Video Tokenization**](<https://proceedings.mlr.press/v306/atanov26a.html>) | 2026 | ICML | [Code](<https://github.com/apple-aiml-research/ml-videoflextok>) · [Project](<https://videoflextok.epfl.ch/>) · [Models](<https://huggingface.co/EPFL-VILAB/videoflextok_d18_d28>) |
| [**VL-JEPA: Joint Embedding Predictive Architecture for Vision-language**](<https://arxiv.org/abs/2512.10942>) | 2026 | ICLR | — |
| [**CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer**](<https://arxiv.org/abs/2408.06072>) | 2025 | ICLR | [Code](<https://github.com/THUDM/CogVideo>) |
| [**Cosmos World Foundation Model Platform for Physical AI**](<https://arxiv.org/abs/2501.03575>) | 2025 | arXiv | [Code](<https://github.com/nvidia-cosmos/cosmos-predict1>) · [Project](<https://research.nvidia.com/labs/dir/cosmos1/>) |
| [**Larp: Tokenizing videos with a learned autoregressive generative prior**](<https://arxiv.org/abs/2410.21264>) | 2025 | ICLR | — |
| [**Learning adaptive and temporally causal video tokenization in a 1d latent space**](<https://arxiv.org/abs/2505.17011>) | 2025 | arXiv | [Code](<https://github.com/VisionXLab/AdapTok>) |
| [**Perception encoder: The best visual embeddings are not at the output of the network**](<https://arxiv.org/abs/2504.13181>) | 2025 | arXiv | [Code](<https://github.com/facebookresearch/perception_models>) |
| [**Siglip 2: Multilingual vision-language encoders with improved semantic understanding, localization, and dense features**](<https://arxiv.org/abs/2502.14786>) | 2025 | arXiv | [Code](<https://github.com/google-research/big_vision/tree/main/big_vision/configs/proj/image_text/README_siglip2.md>) · [Project](<https://github.com/google-research/big_vision/blob/main/big_vision/configs/proj/image_text/README_siglip2.md>) |
| [**V-JEPA~2: Self-Supervised Video Models Enable Understanding, Prediction and Planning**](<https://arxiv.org/abs/2506.09985>) | 2025 | arXiv | [Code](<https://github.com/facebookresearch/vjepa2>) |
| [**VideoVAE+: Large Motion Video Autoencoding with Cross-modal Video VAE**](<https://arxiv.org/abs/2412.17805>) | 2025 | ICCV | [Code](<https://github.com/VideoVerses/VideoVAEPlus>) · [Project](<https://yzxing87.github.io/vae/>) |
| [**Cv-vae: A compatible video vae for latent generative video models**](<https://arxiv.org/abs/2405.20279>) | 2024 | NeurIPS | [Code](<https://github.com/ailab-cvc/cv-vae>) · [Project](<https://ailab-cvc.github.io/cvvae/index.html>) |
| [**InternVid: A Large-Scale Video-Text Dataset for Multimodal Understanding and Generation**](<https://arxiv.org/abs/2307.06942>) | 2024 | ICLR | [Code](<https://github.com/OpenGVLab/InternVideo/tree/main/Data/InternVid>) |
| [**InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks**](<https://arxiv.org/abs/2312.14238>) | 2024 | CVPR | [Code](<https://github.com/opengvlab/internvl>) · [Demo](<https://huggingface.co/spaces/OpenGVLab/InternVL>) |
| [**Language Model Beats Diffusion -- Tokenizer is Key to Visual Generation**](<https://arxiv.org/abs/2310.05737>) | 2024 | ICLR | [Project](<https://magvit.cs.cmu.edu/v2/>) |
| [**Revisiting Feature Prediction for Learning Visual Representations from Video**](<https://arxiv.org/abs/2404.08471>) | 2024 | Transactions on Machine Learning Research | [Code](<https://github.com/facebookresearch/jepa>) · [Project](<https://ai.meta.com/blog/v-jepa-yann-lecun-ai-model-video-joint-embedding-predictive-architecture/>) |
| [**Vidtok: A versatile and open-source video tokenizer**](<https://arxiv.org/abs/2412.13061>) | 2024 | arXiv | [Code](<https://github.com/microsoft/VidTok>) |
| [**Sigmoid Loss for Language Image Pre-Training**](<https://arxiv.org/abs/2303.15343>) | 2023 | ICCV | [Code](<https://github.com/google-research/big_vision>) |
| [**High-Resolution Image Synthesis with Latent Diffusion Models**](<https://doi.org/10.1109/CVPR52688.2022.01042>) | 2022 | CVPR | [Code](<https://github.com/CompVis/latent-diffusion>) |
| [**Taming Transformers for High-Resolution Image Synthesis**](<https://doi.org/10.1109/CVPR46437.2021.01268>) | 2021 | CVPR | [Code](<https://github.com/CompVis/taming-transformers>) |
| [**VideoGPT: Video Generation using VQ-VAE and Transformers**](<https://arxiv.org/abs/2104.10157>) | 2021 | arXiv | [Code](<https://github.com/wilson1yan/VideoGPT>) · [Project](<https://wilson1yan.github.io/videogpt/index.html>) |

#### Joint Audio-Video Tokenization

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**AVTok: 1D Unified Tokenization for Holistic Audio-Video Generation**](<https://arxiv.org/abs/2606.30811>) | 2026 | ECCV | [Code](<https://github.com/hkust-longgroup/AVTok>) · [Project](<https://hkust-longgroup.github.io/AVTok/>) |
| [**JavisDiT: Joint Audio-Video Diffusion Transformer with Hierarchical Spatio-Temporal Prior Synchronization**](<https://arxiv.org/abs/2503.23377>) | 2026 | ICLR | [Code](<https://github.com/JavisVerse/JavisDiT>) · [Project](<https://javisverse.github.io/JavisDiT-page/>) · [Data](<https://huggingface.co/datasets/JavisVerse/JavisBench>) |
| [**MJEPA: A Simple and Scalable Joint-Embedding Predictive Architecture for Audio-Visual Learning**](<https://arxiv.org/abs/2606.25225>) | 2026 | arXiv | [Code](<https://github.com/facebookresearch/MJEPA>) |
| [**Pushing the Frontier of Audiovisual Perception with Large-Scale Multimodal Correspondence Learning**](<https://openaccess.thecvf.com/content/CVPR2026/html/Vyas_Pushing_the_Frontier_of_Audiovisual_Perception_with_Large-Scale_Multimodal_Correspondence_CVPR_2026_paper.html>) | 2026 | CVPR | [Code](<https://github.com/facebookresearch/perception_models>) · [Project](<https://ai.meta.com/research/publications/pushing-the-frontier-of-audiovisual-perception-with-large-scale-multimodal-correspondence-learning/>) · [Models](<https://huggingface.co/facebook/pe-a-frame-base>) |
| [**UniAVGen: Unified Audio and Video Generation with Asymmetric Cross-Modal Interactions**](<https://arxiv.org/abs/2511.03334>) | 2026 | CVPR | [Code](<https://github.com/mcg-nju/sora2-mini>) · [Project](<https://mcg-nju.github.io/UniAVGen/>) |
| [**Ovi: Twin Backbone Cross-Modal Fusion for Audio-Video Generation**](<https://arxiv.org/abs/2510.01284>) | 2025 | arXiv | [Code](<https://github.com/character-ai/Ovi>) · [Project](<https://aaxwaz.github.io/Ovi>) |
| [**AnyGPT: Unified Multimodal LLM with Discrete Sequence Modeling**](<https://arxiv.org/abs/2402.12226>) | 2024 | arXiv | [Code](<https://github.com/OpenMOSS/AnyGPT>) · [Project](<https://junzhan2000.github.io/AnyGPT.github.io/>) |
| [**AV-Link: Temporally-Aligned Diffusion Features for Cross-Modal Audio-Video Generation**](<https://arxiv.org/abs/2412.15191>) | 2024 | arXiv | [Code](<https://github.com/snap-research/AVLink>) · [Project](<https://snap-research.github.io/AVLink/>) |
| [**LanguageBind: Extending Video-Language Pretraining to N-modality by Language-based Semantic Alignment**](<https://arxiv.org/abs/2310.01852>) | 2024 | ICLR | [Code](<https://github.com/PKU-YuanGroup/LanguageBind>) |
| [**ImageBind: One Embedding Space To Bind Them All**](<https://doi.org/10.1109/cvpr52729.2023.01457>) | 2023 | CVPR | [Code](<https://github.com/facebookresearch/ImageBind>) |
| [**ONE-PEACE: Exploring One General Representation Model Toward Unlimited Modalities**](<https://arxiv.org/abs/2305.11172>) | 2023 | arXiv | [Code](<https://github.com/OFA-Sys/ONE-PEACE>) |

## Awesome Datasets

### Joint Audio-Video Corpora

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**What's Making That Sound Right Now? Video-centric Audio-Visual Localization**](<https://doi.org/10.1109/iccv51701.2025.01869>) | 2025 | ICCV | [Project](<https://hahyeon610.github.io/Video-centric_Audio_Visual_Localization/>) |
| [**Tavgbench: Benchmarking text to audible-video generation**](<https://arxiv.org/abs/2404.14381>) | 2024 | ACM MM | [Code](<https://github.com/opennlplab/tavgbench>) |
| [**Audio-Visual Instance Segmentation**](<https://arxiv.org/abs/2310.18709>) | 2023 | arXiv | [Code](<https://github.com/ruohaoguo/avis>) |
| [**Audio-Visual Segmentation with Semantics**](<https://arxiv.org/abs/2301.13190>) | 2023 | arXiv | [Code](<https://github.com/OpenNLPLab/AVSBench>) |
| [**VALOR: Vision-Audio-Language Omni-Perception Pretraining Model and Dataset**](<https://arxiv.org/abs/2304.08345>) | 2023 | arXiv | [Code](<https://github.com/TXH-mercury/VALOR>) |
| [**Audio-Visual Segmentation**](<https://arxiv.org/abs/2207.05042>) | 2022 | ECCV | [Code](<https://github.com/OpenNLPLab/AVSBench>) |
| [**Learning to Answer Questions in Dynamic Audio-Visual Scenarios**](<https://arxiv.org/abs/2203.14072>) | 2022 | CVPR | [Code](<https://github.com/GeWu-Lab/MUSIC-AVQA>) |
| [**Sound-Guided Semantic Video Generation**](<https://arxiv.org/abs/2204.09273>) | 2022 | ECCV | — |
| [**VGGSound: A Large-scale Audio-Visual Dataset**](<https://arxiv.org/abs/2004.14368>) | 2020 | ICASSP | [Code](<https://github.com/hongliechen/VGGSound>) · [Data](<https://www.robots.ox.ac.uk/~vgg/data/vggsound/>) |
| [**2.5D Visual Sound**](<https://arxiv.org/abs/1812.04204>) | 2019 | CVPR | [Code](<https://github.com/facebookresearch/2.5D-Visual-Sound>) |
| [**Audio Visual Scene-Aware Dialog**](<https://arxiv.org/abs/1901.09107>) | 2019 | CVPR | — |
| [**AudioCaps: Generating Captions for Audios in the Wild**](<https://doi.org/10.18653/v1/N19-1011>) | 2019 | NAACL | [Data](<https://audiocaps.github.io/>) |
| [**How2: A Large-scale Dataset for Multimodal Language Understanding**](<https://nips2018vigil.github.io/static/papers/accepted/26.pdf>) | 2018 | — | — |
| [**The Sound of Pixels**](<https://arxiv.org/abs/1804.03160>) | 2018 | ECCV | [Code](<https://github.com/hangzhaomit/Sound-of-Pixels>) |
| [**Audio Set: An Ontology and Human-Labeled Dataset for Audio Events**](<https://doi.org/10.1109/ICASSP.2017.7952261>) | 2017 | ICASSP | [Data](<https://research.google.com/audioset/>) |
| [**Visually Indicated Sounds**](<https://arxiv.org/abs/1512.08512>) | 2016 | CVPR | — |

### Video Pretraining

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**InternVid: A Large-Scale Video-Text Dataset for Multimodal Understanding and Generation**](<https://arxiv.org/abs/2307.06942>) | 2024 | ICLR | [Code](<https://github.com/OpenGVLab/InternVideo/tree/main/Data/InternVid>) |
| [**Panda-70M: Captioning 70M Videos with Multiple Cross-Modality Teachers**](<https://arxiv.org/abs/2402.19479>) | 2024 | CVPR | [Code](<https://github.com/snap-research/panda-70m>) · [Project](<https://snap-research.github.io/Panda-70M>) · [Data](<https://github.com/snap-research/Panda-70M>) |
| [**Advancing High-Resolution Video-Language Representation with Large-Scale Video Transcriptions**](<https://arxiv.org/abs/2111.10337>) | 2022 | CVPR | [Code](<https://github.com/microsoft/XPretrain/tree/main/hd-vila-100m>) |
| [**Frozen in Time: A Joint Video and Image Encoder for End-to-End Retrieval**](<https://doi.org/10.1109/ICCV48922.2021.00175>) | 2021 | ICCV | [Code](<https://github.com/m-bain/frozen-in-time>) |
| [**The Kinetics Human Action Video Dataset**](<https://arxiv.org/abs/1705.06950>) | 2017 | arXiv | [Data](<https://www.robots.ox.ac.uk/~vgg/data/kinetics/>) |
| [**ActivityNet: A Large-Scale Video Benchmark for Human Activity Understanding**](<https://openaccess.thecvf.com/content_cvpr_2015/html/Caba_Heilbron_ActivityNet_A_Large-Scale_2015_CVPR_paper.html>) | 2015 | CVPR | [Data](<http://activity-net.org/>) |
| [**UCF101: A dataset of 101 human actions classes from videos in the wild**](<https://arxiv.org/abs/1212.0402>) | 2012 | arXiv | [Data](<https://www.crcv.ucf.edu/data/UCF101.php>) |

### Audio Pretraining

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**WavCaps: A ChatGPT-Assisted Weakly-Labelled Audio Captioning Dataset for Audio-Language Multimodal Research**](<https://arxiv.org/abs/2303.17395>) | 2024 | IEEE/ACM Transactions on Audio, Speech, and Language Processing | [Code](<https://github.com/xinhaomei/wavcaps>) · [Data](<https://huggingface.co/datasets/cvssp/WavCaps>) |
| [**GigaSpeech: An Evolving, Multi-domain ASR Corpus with 10,000 Hours of Transcribed Audio**](<https://doi.org/10.21437/interspeech.2021-1965>) | 2021 | Interspeech | [Code](<https://github.com/SpeechColab/GigaSpeech>) · [Data](<https://huggingface.co/datasets/speechcolab/gigaspeech>) |
| [**Libri-Light: A Benchmark for ASR with Limited or No Supervision**](<https://arxiv.org/abs/1912.07875>) | 2020 | ICASSP | [Code](<https://github.com/facebookresearch/libri-light>) |
| [**Audio Set: An Ontology and Human-Labeled Dataset for Audio Events**](<https://doi.org/10.1109/ICASSP.2017.7952261>) | 2017 | ICASSP | [Data](<https://research.google.com/audioset/>) |
| [**LibriSpeech: An ASR Corpus Based on Public Domain Audio Books**](<https://doi.org/10.1109/ICASSP.2015.7178964>) | 2015 | ICASSP | [Data](<https://www.openslr.org/12>) |
| [**Evaluation of Algorithms Using Games: The Case of Music Tagging**](<https://ismir2009.ismir.net/proceedings/OS5-5.pdf>) | 2009 | Proc. International Society for Music Information Retrieval Conference (ISMIR) | — |

## Awesome Benchmarks and Metrics

### Benchmarks

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**JavisDiT: Joint Audio-Video Diffusion Transformer with Hierarchical Spatio-Temporal Prior Synchronization**](<https://arxiv.org/abs/2503.23377>) | 2026 | ICLR | [Code](<https://github.com/JavisVerse/JavisDiT>) · [Project](<https://javisverse.github.io/JavisDiT-page/>) · [Data](<https://huggingface.co/datasets/JavisVerse/JavisBench>) |
| [**T2AV-Compass: Towards Unified Evaluation for Text-to-Audio-Video Generation**](<https://proceedings.mlr.press/v306/cao26v.html>) | 2026 | ICML | — |
| [**WorldSense: Evaluating Real-world Omnimodal Understanding for Multimodal LLMs**](<https://arxiv.org/abs/2502.04326>) | 2026 | ICLR | [Project](<https://jaaackhongggg.github.io/WorldSense>) |
| [**Daily-Omni: Towards Audio-Visual Reasoning with Temporal Alignment across Modalities**](<https://arxiv.org/abs/2505.17862>) | 2025 | arXiv | — |
| [**FoleyBench: A Benchmark For Video-to-Audio Models**](<https://arxiv.org/abs/2511.13219>) | 2025 | arXiv | — |
| [**OmniBench: Towards The Future of Universal Omni-Language Models**](<https://doi.org/10.52202/085713-1036>) | 2025 | NeurIPS | [Code](<https://github.com/m-a-p/OmniBench>) |
| [**OmniVideoBench: Towards Audio-Visual Understanding Evaluation for Omni MLLMs**](<https://arxiv.org/abs/2510.10689>) | 2025 | arXiv | [Code](<https://github.com/NJU-LINK/OmniVideoBench>) · [Project](<https://omnivideobench.github.io/omnivideobench_home/>) |
| [**SpA2V: Harnessing Spatial Auditory Cues for Audio-driven Spatially-aware Video Generation**](<https://arxiv.org/abs/2508.00782>) | 2025 | ACM MM | — |
| [**What's Making That Sound Right Now? Video-centric Audio-Visual Localization**](<https://doi.org/10.1109/iccv51701.2025.01869>) | 2025 | ICCV | [Project](<https://hahyeon610.github.io/Video-centric_Audio_Visual_Localization/>) |
| [**AV-Odyssey Bench: Can Your Multimodal LLMs Really Understand Audio-Visual Information?**](<https://arxiv.org/abs/2412.02611>) | 2024 | arXiv | [Code](<https://github.com/av-odyssey/av-odyssey>) · [Project](<https://av-odyssey.github.io/>) · [Demo](<https://huggingface.co/spaces/AV-Odyssey/AV_Odyssey_Bench_Leaderboard>) |
| [**EvalCrafter: Benchmarking and Evaluating Large Video Generation Models**](<https://doi.org/10.1109/CVPR52733.2024.02090>) | 2024 | CVPR | — |
| [**Tavgbench: Benchmarking text to audible-video generation**](<https://arxiv.org/abs/2404.14381>) | 2024 | ACM MM | [Code](<https://github.com/opennlplab/tavgbench>) |
| [**VBench: Comprehensive Benchmark Suite for Video Generative Models**](<https://arxiv.org/abs/2311.17982>) | 2024 | CVPR | [Code](<https://github.com/vchitect/vbench>) · [Demo](<https://huggingface.co/spaces/Vchitect/VBench>) |
| [**Audio-Visual Segmentation with Semantics**](<https://arxiv.org/abs/2301.13190>) | 2023 | arXiv | [Code](<https://github.com/OpenNLPLab/AVSBench>) |
| [**Audio-Visual Segmentation**](<https://arxiv.org/abs/2207.05042>) | 2022 | ECCV | [Code](<https://github.com/OpenNLPLab/AVSBench>) |
| [**Learning to Answer Questions in Dynamic Audio-Visual Scenarios**](<https://arxiv.org/abs/2203.14072>) | 2022 | CVPR | [Code](<https://github.com/GeWu-Lab/MUSIC-AVQA>) |
| [**Unified Multisensory Perception: Weakly-Supervised Audio-Visual Video Parsing**](<https://doi.org/10.1007/978-3-030-58580-8_26>) | 2020 | ECCV | [Code](<https://github.com/YapengTian/AVVP-ECCV20>) |
| [**VGGSound: A Large-scale Audio-Visual Dataset**](<https://arxiv.org/abs/2004.14368>) | 2020 | ICASSP | [Code](<https://github.com/hongliechen/VGGSound>) · [Data](<https://www.robots.ox.ac.uk/~vgg/data/vggsound/>) |
| [**Audio Visual Scene-Aware Dialog**](<https://arxiv.org/abs/1901.09107>) | 2019 | CVPR | — |
| [**AudioCaps: Generating Captions for Audios in the Wild**](<https://doi.org/10.18653/v1/N19-1011>) | 2019 | NAACL | [Data](<https://audiocaps.github.io/>) |
| [**Audio-Visual Event Localization in Unconstrained Videos**](<https://doi.org/10.1007/978-3-030-01216-8_16>) | 2018 | ECCV | [Code](<https://github.com/YapengTian/AVE-ECCV18>) |

### Metrics

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**JavisDiT: Joint Audio-Video Diffusion Transformer with Hierarchical Spatio-Temporal Prior Synchronization**](<https://arxiv.org/abs/2503.23377>) | 2026 | ICLR | [Code](<https://github.com/JavisVerse/JavisDiT>) · [Project](<https://javisverse.github.io/JavisDiT-page/>) · [Data](<https://huggingface.co/datasets/JavisVerse/JavisBench>) |
| [**Meta Audiobox Aesthetics: Unified Automatic Quality Assessment for Speech, Music, and Sound**](<https://arxiv.org/abs/2502.05139>) | 2025 | arXiv | [Code](<https://github.com/facebookresearch/audiobox-aesthetics>) |
| [**Syncphony: Synchronized Audio-to-Video Generation with Diffusion Transformers**](<https://arxiv.org/abs/2509.21893>) | 2025 | arXiv | [Project](<https://jibin86.github.io/syncphony_project_page>) |
| [**Audio-Synchronized Visual Animation**](<https://arxiv.org/abs/2403.05659>) | 2024 | ECCV | — |
| [**Diverse and Aligned Audio-to-Video Generation via Text-to-Video Model Adaptation**](<https://ojs.aaai.org/index.php/AAAI/article/view/28486>) | 2024 | AAAI | — |
| [**Synchformer: Efficient synchronization from sparse cues**](<https://doi.org/10.1109/icassp48485.2024.10448489>) | 2024 | ICASSP | [Code](<https://github.com/v-iashin/Synchformer>) |
| [**Exploring Video Quality Assessment on User Generated Contents from Aesthetic and Technical Perspectives**](<https://arxiv.org/abs/2211.04894>) | 2023 | ICCV | — |
| [**ImageBind: One Embedding Space To Bind Them All**](<https://doi.org/10.1109/cvpr52729.2023.01457>) | 2023 | CVPR | [Code](<https://github.com/facebookresearch/ImageBind>) |
| [**Large-Scale Contrastive Language-Audio Pretraining with Feature Fusion and Keyword-to-Caption Augmentation**](<https://doi.org/10.1109/icassp49357.2023.10095969>) | 2023 | ICASSP | [Code](<https://github.com/laion-ai/clap>) |
| [**AudioCLIP: Extending CLIP to Image, Text and Audio**](<https://doi.org/10.1109/ICASSP43922.2022.9747631>) | 2022 | ICASSP | [Code](<https://github.com/AndreyGuzhov/AudioCLIP>) |
| [**LAION-Aesthetics**](<https://laion.ai/blog/laion-aesthetics/>) | 2022 | — | — |
| [**Learning Transferable Visual Models From Natural Language Supervision**](<https://arxiv.org/abs/2103.00020>) | 2021 | ICML | [Code](<https://github.com/openai/CLIP>) |
| [**NISQA: A deep CNN-self-attention model for multidimensional speech quality prediction with crowdsourced datasets**](<https://arxiv.org/abs/2104.09494>) | 2021 | arXiv | [Code](<https://github.com/gabrielmittag/NISQA>) |
| [**A Lip Sync Expert Is All You Need for Speech to Lip Generation In the Wild**](<https://arxiv.org/abs/2008.10010>) | 2020 | ACM MM | [Code](<https://github.com/Rudrabha/Wav2Lip>) |
| [**Fréchet Audio Distance: A Reference-Free Metric for Evaluating Music Enhancement Algorithms**](<https://doi.org/10.21437/Interspeech.2019-2219>) | 2019 | Interspeech | [Code](<https://github.com/google-research/google-research/tree/master/frechet_audio_distance>) |
| [**FVD: A New Metric for Video Generation**](<https://arxiv.org/abs/1812.01717>) | 2019 | ICLR Workshop on Deep Generative Models for Highly Structured Data | [Code](<https://github.com/google-research/google-research/tree/master/frechet_video_distance>) |
| [**The Unreasonable Effectiveness of Deep Features as a Perceptual Metric**](<https://arxiv.org/abs/1801.03924>) | 2018 | CVPR | [Code](<https://github.com/richzhang/PerceptualSimilarity>) · [Project](<https://richzhang.github.io/PerceptualSimilarity/>) |
| [**GANs Trained by a Two Time-Scale Update Rule Converge to a Local Nash Equilibrium**](<https://arxiv.org/abs/1706.08500>) | 2017 | NeurIPS | [Code](<https://github.com/bioinf-jku/TTUR>) |
| [**Out of Time: Automated Lip Sync in the Wild**](<https://doi.org/10.1007/978-3-319-54427-4_19>) | 2017 | ACCV Workshops | [Code](<https://github.com/joonson/syncnet_python>) · [Project](<https://www.robots.ox.ac.uk/~vgg/software/lipsync/>) |
| [**Improved Techniques for Training GANs**](<https://arxiv.org/abs/1606.03498>) | 2016 | NeurIPS | [Code](<https://github.com/openai/improved-gan>) |
| [**CIDEr: Consensus-based Image Description Evaluation**](<https://arxiv.org/abs/1411.5726>) | 2015 | CVPR | — |
| [**A Short-Time Objective Intelligibility Measure for Time-Frequency Weighted Noisy Speech**](<https://doi.org/10.1109/ICASSP.2010.5495701>) | 2010 | ICASSP | — |
| [**METEOR: An Automatic Metric for MT Evaluation with Improved Correlation with Human Judgments**](<https://aclanthology.org/W05-0909/>) | 2005 | ACL Workshop | — |
| [**Image quality assessment: from error visibility to structural similarity**](<https://doi.org/10.1109/tip.2003.819861>) | 2004 | IEEE Transactions on Image Processing | — |
| [**BLEU: A Method for Automatic Evaluation of Machine Translation**](<https://aclanthology.org/P02-1040/>) | 2002 | ACL | — |
| [**Perceptual evaluation of speech quality (PESQ)-a new method for speech quality assessment of telephone networks and codecs**](<https://doi.org/10.1109/ICASSP.2001.941023>) | 2001 | ICASSP | — |

## Related Work and Foundations

| Title | Year | Venue | Resources |
|:--|:--:|:--|:--|
| [**Audio-Visual Intelligence in Large Foundation Models**](<https://arxiv.org/abs/2605.04045>) | 2026 | arXiv | [GitHub](<https://github.com/JavisVerse/Awesome-AVI>) |
| [**From Specific-MLLMs to Omni-MLLMs: A Survey on MLLMs Aligned with Multi-modalities**](<https://aclanthology.org/2025.findings-acl.453/>) | 2025 | Findings of the Association for Computational Linguistics: ACL 2025 | — |
| [**From Waveforms to Pixels: A Survey on Audio-Visual Segmentation**](<https://arxiv.org/abs/2508.03724>) | 2025 | arXiv | — |
| [**Scaling Laws for Native Multimodal Models**](<https://arxiv.org/abs/2504.07951>) | 2025 | ICCV | [Project](<https://machinelearning.apple.com/research/scaling-laws-native-multimodal-models>) |
| [**Towards Holistic Evaluation of Large Audio-Language Models: A Comprehensive Survey**](<https://doi.org/10.18653/v1/2025.emnlp-main.514>) | 2025 | Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing | — |
| [**Towards Precise Scaling Laws for Video Diffusion Transformers**](<https://openaccess.thecvf.com/content/CVPR2025/html/Yin_Towards_Precise_Scaling_Laws_for_Video_Diffusion_Transformers_CVPR_2025_paper.html>) | 2025 | CVPR | — |
| [**Unified Multimodal Understanding and Generation Models: Advances, Challenges, and Opportunities**](<https://arxiv.org/abs/2505.02567>) | 2025 | arXiv | [GitHub](<https://github.com/aidc-ai/awesome-unified-multimodal-models>) |
| [**A survey on multimodal large language models**](<http://dx.doi.org/10.1093/nsr/nwae403>) | 2024 | National Science Review | — |
| [**A Survey on Video Diffusion Models**](<https://arxiv.org/abs/2310.10647>) | 2024 | arXiv | [GitHub](<https://github.com/ChenHsing/Awesome-Video-Diffusion-Models>) |
| [**Generative Multimodal Models are In-Context Learners**](<https://arxiv.org/abs/2312.13286>) | 2024 | CVPR | [Code](<https://github.com/baaivision/emu>) · [Project](<https://baaivision.github.io/emu2>) |
| [**LLMs Meet Multimodal Generation and Editing: A Survey**](<https://arxiv.org/abs/2405.19334>) | 2024 | arXiv | — |
| [**OmniFlow: Any-to-Any Generation with Multi-Modal Rectified Flows**](<https://arxiv.org/abs/2412.01169>) | 2024 | arXiv | [Code](<https://github.com/jacklishufan/OmniFlows>) |
| [**Scaling Rectified Flow Transformers for High-Resolution Image Synthesis**](<https://arxiv.org/abs/2403.03206>) | 2024 | arXiv | — |
| [**SiT: Exploring Flow and Diffusion-based Generative Models with Scalable Interpolant Transformers**](<https://arxiv.org/abs/2401.08740>) | 2024 | ECCV | [Code](<https://github.com/willisma/sit>) |
| [**The Revolution of Multimodal Large Language Models: A Survey**](<https://aclanthology.org/2024.findings-acl.807/>) | 2024 | Findings of the Association for Computational Linguistics: ACL 2024 | — |
| [**Video Generation Models as World Simulators**](<https://openai.com/index/video-generation-models-as-world-simulators/>) | 2024 | — | — |
| [**A Survey on Audio Diffusion Models: Text To Speech Synthesis and Enhancement in Generative AI**](<https://arxiv.org/abs/2303.13336>) | 2023 | arXiv | — |
| [**Audio-Visual Grouping Network for Sound Localization from Mixtures**](<https://doi.org/10.1109/CVPR52729.2023.01018>) | 2023 | CVPR | [Code](<https://github.com/stoneMo/AVGN>) |
| [**AudioLDM: Text-to-Audio Generation with Latent Diffusion Models**](<https://proceedings.mlr.press/v202/liu23f.html>) | 2023 | ICML | — |
| [**AudioLM: A Language Modeling Approach to Audio Generation**](<https://doi.org/10.1109/TASLP.2023.3288409>) | 2023 | IEEE/ACM Trans. Audio, Speech, Language Process. | — |
| [**BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models**](<https://proceedings.mlr.press/v202/li23q.html>) | 2023 | ICML | [Code](<https://github.com/salesforce/LAVIS/tree/main/projects/blip2>) |
| [**Consistency Models**](<https://arxiv.org/abs/2303.01469>) | 2023 | ICML | [Code](<https://github.com/openai/consistency_models>) |
| [**EVA-CLIP: Improved Training Techniques for CLIP at Scale**](<https://arxiv.org/abs/2303.15389>) | 2023 | arXiv | [Code](<https://github.com/baaivision/EVA/tree/master/EVA-CLIP>) |
| [**Fine-grained Audio-Visual Joint Representations for Multimodal Large Language Models**](<https://arxiv.org/abs/2310.05863>) | 2023 | arXiv | [Code](<https://github.com/BriansIDP/AudioVisualLLM.git>) |
| [**Flow Matching for Generative Modeling**](<https://openreview.net/forum?id=PqvMRDCJT9t>) | 2023 | ICLR | — |
| [**Flow Straight and Fast: Learning to Generate and Transfer Data with Rectified Flow**](<https://arxiv.org/abs/2209.03003>) | 2023 | ICLR | — |
| [**LLaMA: Open and Efficient Foundation Language Models**](<https://arxiv.org/abs/2302.13971>) | 2023 | arXiv | — |
| [**Make-A-Video: Text-to-Video Generation without Text-Video Data**](<https://arxiv.org/abs/2209.14792>) | 2023 | ICLR | [Project](<https://makeavideo.studio/>) |
| [**Qwen: Technical Report**](<https://arxiv.org/abs/2309.16609>) | 2023 | arXiv | [Code](<https://github.com/QwenLM/Qwen-7B>) |
| [**Scalable Diffusion Models with Transformers**](<https://arxiv.org/abs/2212.09748>) | 2023 | ICCV | [Code](<https://github.com/facebookresearch/DiT>) · [Project](<https://www.wpeebles.com/DiT>) |
| [**Simple and Controllable Music Generation**](<https://doi.org/10.52202/075280-2066>) | 2023 | NeurIPS | [Code](<https://github.com/facebookresearch/audiocraft>) |
| [**SoundStorm: Efficient Parallel Audio Generation**](<https://arxiv.org/abs/2305.09636>) | 2023 | arXiv | [Project](<https://google-research.github.io/seanet/soundstorm/examples/>) |
| [**VALL-E: Neural Codec Language Models are Zero-Shot Text to Speech Synthesizers**](<https://arxiv.org/abs/2301.02111>) | 2023 | arXiv | — |
| [**Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%* ChatGPT Quality**](<https://lmsys.org/blog/2023-03-30-vicuna/>) | 2023 | — | [Code](<https://github.com/lm-sys/FastChat>) · [Demo](<https://chat.lmsys.org/>) |
| [**Visual Instruction Tuning**](<https://arxiv.org/abs/2304.08485>) | 2023 | NeurIPS | [Code](<https://github.com/haotian-liu/LLaVA>) · [Project](<https://llava-vl.github.io/>) |
| [**A Path Towards Autonomous Machine Intelligence**](<https://openreview.net/forum?id=BZ5a1r-kVsf>) | 2022 | — | — |
| [**Classifier-Free Diffusion Guidance**](<https://arxiv.org/abs/2207.12598>) | 2022 | arXiv | — |
| [**Flamingo: A Visual Language Model for Few-Shot Learning**](<https://arxiv.org/abs/2204.14198>) | 2022 | NeurIPS | — |
| [**FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness**](<https://doi.org/10.52202/068431-1189>) | 2022 | NeurIPS | [Code](<https://github.com/Dao-AILab/flash-attention>) |
| [**Masked Autoencoders Are Scalable Vision Learners**](<https://doi.org/10.1109/CVPR52688.2022.01553>) | 2022 | CVPR | [Code](<https://github.com/facebookresearch/mae>) |
| [**Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding**](<https://arxiv.org/abs/2205.11487>) | 2022 | NeurIPS | [Project](<https://imagen.research.google/>) |
| [**VideoMAE: Masked Autoencoders are Data-Efficient Learners for Self-Supervised Video Pre-Training**](<https://arxiv.org/abs/2203.12602>) | 2022 | NeurIPS | [Code](<https://github.com/MCG-NJU/VideoMAE>) |
| [**An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale**](<https://arxiv.org/abs/2010.11929>) | 2021 | ICLR | [Code](<https://github.com/google-research/vision_transformer>) |
| [**Denoising Diffusion Implicit Models**](<https://arxiv.org/abs/2010.02502>) | 2021 | ICLR | [Code](<https://github.com/ermongroup/ddim>) |
| [**QuerYD: A Video Dataset with High-Quality Text and Audio Narrations**](<https://doi.org/10.1109/ICASSP39728.2021.9414640>) | 2021 | ICASSP | — |
| [**Score-Based Generative Modeling through Stochastic Differential Equations**](<https://arxiv.org/abs/2011.13456>) | 2021 | ICLR | [Code](<https://github.com/yang-song/score_sde>) |
| [**Denoising Diffusion Probabilistic Models**](<https://arxiv.org/abs/2006.11239>) | 2020 | NeurIPS | [Code](<https://github.com/hojonathanho/diffusion>) |
| [**Language Models are Few-Shot Learners**](<https://arxiv.org/abs/2005.14165>) | 2020 | NeurIPS | [Code](<https://github.com/openai/gpt-3>) |
| [**PANNs: Large-Scale Pretrained Audio Neural Networks for Audio Pattern Recognition**](<https://arxiv.org/abs/1912.10211>) | 2020 | IEEE/ACM Trans. Audio, Speech, Language Process. | [Code](<https://github.com/qiuqiangkong/audioset_tagging_cnn>) |
| [**Scaling Laws for Neural Language Models**](<https://arxiv.org/abs/2001.08361>) | 2020 | arXiv | — |
| [**Language Models are Unsupervised Multitask Learners**](<https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf>) | 2019 | OpenAI | [Code](<https://github.com/openai/gpt-2>) · [Project](<https://openai.com/index/better-language-models/>) |
| [**The Bitter Lesson**](<http://www.incompleteideas.net/IncIdeas/BitterLesson.html>) | 2019 | — | — |
| [**Neural Ordinary Differential Equations**](<https://arxiv.org/abs/1806.07366>) | 2018 | NeurIPS | [Code](<https://github.com/rtqichen/torchdiffeq>) |
| [**Self-Supervised Generation of Spatial Audio for 360 Video**](<https://arxiv.org/abs/1809.02540>) | 2018 | NeurIPS | — |
| [**Attention Is All You Need**](<https://arxiv.org/abs/1706.03762>) | 2017 | NeurIPS | [Code](<https://github.com/tensorflow/tensor2tensor>) |
| [**CNN Architectures for Large-Scale Audio Classification**](<https://arxiv.org/abs/1609.09430>) | 2017 | ICASSP | [Code](<https://github.com/tensorflow/models/tree/master/research/audioset/vggish>) |
| [**Neural Discrete Representation Learning**](<https://arxiv.org/abs/1711.00937>) | 2017 | NeurIPS | [Code](<https://github.com/deepmind/sonnet/blob/v2/sonnet/src/nets/vqvae.py>) |
| [**SampleRNN: An Unconditional End-to-End Neural Audio Generation Model**](<https://arxiv.org/abs/1612.07837>) | 2017 | ICLR | [Code](<https://github.com/soroushmehr/sampleRNN_ICLR2017>) |
| [**WaveNet: A Generative Model for Raw Audio**](<https://arxiv.org/abs/1609.03499>) | 2016 | arXiv | — |
| [**Deep Unsupervised Learning using Nonequilibrium Thermodynamics**](<https://arxiv.org/abs/1503.03585>) | 2015 | ICML | [Code](<https://github.com/Sohl-Dickstein/Diffusion-Probabilistic-Models>) |
| [**U-Net: Convolutional Networks for Biomedical Image Segmentation**](<https://doi.org/10.1007/978-3-319-24574-4_28>) | 2015 | MICCAI | — |
| [**Auto-Encoding Variational Bayes**](<https://arxiv.org/abs/1312.6114>) | 2014 | ICLR | — |
<!-- catalog:end -->

## Acknowledgements

The layout takes inspiration from [Awesome-Multimodal-Large-Language-Models](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models). The entries and categories come from our survey.

## BibTeX

If this survey is useful to your work, please cite it. For an individual model, dataset, or benchmark, cite the original work listed in its table.

```bibtex
@misc{pham2026unifiedav,
  title={Unifying Audio-Video Understanding and Generation: Foundations, Taxonomies, and Architectures},
  author={Pham, Kien T. and He, Zhenqi and Wang, Yanghao and Chen, Qifeng and Chen, Long},
  year={2026},
  note={Survey manuscript}
}
```
