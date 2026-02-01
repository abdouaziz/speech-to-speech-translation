# THE COMPREHENSIVE ASR READING LIST (2006–2026)


### Neural ASR Foundations (The Pre-SSL Era)
Before representation learning, these papers established the loss functions and architectures that allow us to train speech models without complex phonetic alignments.

*   **[Classic] Connectionist Temporal Classification (CTC)** (Graves et al., 2006)  
    [https://dl.acm.org/doi/10.1145/1143844.1143891](https://dl.acm.org/doi/10.1145/1143844.1143891)  
    *The backbone of modern ASR (Whisper, wav2vec 2.0, USM). It solved the problem of mapping variable-length audio to variable-length text.*

*   **[1512.02595] Deep Speech 2: End-to-End Speech Recognition in English and Mandarin** (2015)  
    [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595)  
    *Baidu's landmark paper on scaling: It proved that large RNNs with simple CTC loss could outperform traditional HMM-GMM pipelines.*

*   **[1508.01211] Listen, Attend and Spell (LAS)** (2016)  
    [https://arxiv.org/abs/1508.01211](https://arxiv.org/abs/1508.01211)  
    *Introduced the Attention mechanism to ASR, moving away from CTC toward a pure sequence-to-sequence framework.*

*   **[1809.08895] Speech-Transformer: A No-Recurrence Sequence-to-Sequence Model** (2018)  
    [https://arxiv.org/abs/1809.08895](https://arxiv.org/abs/1809.08895)  
    *The direct ancestor of modern ASR decoders, applying the "Attention Is All You Need" architecture to speech.*


### Foundations of Self-Supervised Learning (SSL)
These papers define the "Representation Learning" era, where we learn what speech "sounds like" using massive unlabeled datasets.

*   **[1807.03748] Representation Learning with Contrastive Predictive Coding (CPC)** (2018)  
    [https://arxiv.org/abs/1807.03748](https://arxiv.org/abs/1807.03748)  
    *The "Big Bang" of SSL. Introduced the InfoNCE loss for predicting future speech frames in a latent space.*

*   **[2006.11477] wav2vec 2.0: A Framework for Self-Supervised Learning** (2020)  
    [https://arxiv.org/abs/2006.11477](https://arxiv.org/abs/2006.11477)  
    *The standard-bearer for SSL. Introduced masked prediction of quantized speech units.*

*   **[2106.07447] HuBERT: Hidden-Unit BERT for Self-Supervised Speech Learning** (2021)  
    [https://arxiv.org/abs/2106.07447](https://arxiv.org/abs/2106.07447)  
    *A shift toward "pseudo-labeling" via clustering, resulting in much cleaner phonetic representations than wav2vec 2.0.*

*   **[2110.13900] WavLM: Large-Scale Pre-Training for Full Stack Speech Processing** (2021)  
    [https://arxiv.org/abs/2110.13900](https://arxiv.org/abs/2110.13900)  
    *Combined HuBERT-style masked prediction with a denoising task to handle noise and overlapping speakers.*

*   **[2202.03555] Data2vec: A General Framework for SSL across Speech, Vision, and Text** (2022)  
    [https://arxiv.org/abs/2202.03555](https://arxiv.org/abs/2202.03555)  
    *Meta AI's move toward a unified SSL methodology using a teacher-student distillation approach.*


### Architecture Optimization & The Conformer
Crucial for understanding how to build a state-of-the-art ASR encoder.

*   **[2005.08100] Conformer: Convolution-augmented Transformer for Speech Recognition** (2020)  
    [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100)  
    *Critical: Combines Convolutions (local context) and Transformers (global context). Used in Google USM, NVIDIA Canary, and SeamlessM4T.*


### Large-Scale Scaling & Multilingualism
This era leverages web-scale data and focuses on bringing ASR to all the world's languages.

*   **[2212.04356] Robust Speech Recognition via Large-Scale Weak Supervision (Whisper)** (2022)  
    [https://arxiv.org/abs/2212.04356](https://arxiv.org/abs/2212.04356)  
    *OpenAI's proof that 680k hours of "weakly labeled" data is more robust than any lab-grown model.*

*   **[2303.01037] Google USM: Scaling Automatic Speech Recognition Beyond 100 Languages** (2023)  
    [https://arxiv.org/abs/2303.01037](https://arxiv.org/abs/2303.01037)  
    *Scaling ASR to 12 million hours using a 2-billion parameter Conformer and BEST-RQ pre-training.*

*   **[2305.13516] Scaling Speech Technology to 1,000+ Languages (Meta MMS)** (2023)  
    [https://arxiv.org/abs/2305.13516](https://arxiv.org/abs/2305.13516)  
    *Critical for low-resource ASR, demonstrating how SSL (wav2vec 2.0) can scale ASR to thousands of languages with minimal data.*


### LLM-Integrated ASR & The "Omni" Era (2024–2026)
Current research integrates ASR into Large Language Models to enable "reasoning" about audio.

*   **[2501.07166] Qwen2-Audio: Empowering Languages with Large-scale Audio Pre-training** (2025)  
    [https://arxiv.org/abs/2501.07166](https://arxiv.org/abs/2501.07166)  
    *Alibaba's latest "Omni" model showing how to plug speech encoders directly into a large LLM for high-accuracy ASR.*

*   **[2506.11160] S2ST-Omni / Qwen3-Speech Technical Preview** (2025/2026)  
    [https://arxiv.org/abs/2506.11160](https://arxiv.org/abs/2506.11160)  
    *Explores hierarchical language-aware adaptation for Speech-LLMs, focusing on state-of-the-art transcription.*

*   **[2508.15827] Mini-Omni-Reasoner: Token-Level Thinking-in-Speaking in Large Speech Models** (2025/2026)  
    [https://arxiv.org/abs/2508.15827](https://arxiv.org/abs/2508.15827)  
    *A cutting-edge look at "Reasoning ASR," where the model "thinks" internally to resolve complex phonetic ambiguities.*


### Evaluation & Surveys
To consolidate your knowledge for your PhD defense.

*   **[2105.01051] SUPERB: Speech processing Universal PERformance Benchmark** (2021)  
    [https://arxiv.org/abs/2105.01051](https://arxiv.org/abs/2105.01051)  
    *The benchmark paper that defined how we evaluate SSL models.*

*   **[2210.08601] Self-Supervised Learning for Speech Processing: A Review** (2022)  
    [https://arxiv.org/abs/2210.08601](https://arxiv.org/abs/2210.08601)  
    *Comprehensive survey of the representational learning era.*

*   **[2410.03058] Large Language Models for Speech Processing: A Survey** (2024)  
    [https://arxiv.org/abs/2410.03058](https://arxiv.org/abs/2410.03058)  
    *The bridge between classical ASR and modern Speech-LLMs.*