# SPEECH-TO-SPEECH TRANSLATION

Here is the updated curated list of key **arXiv papers** on **speech-to-speech translation (S2ST)**, now including a new section on **Cascaded Speech-to-Speech Translation** (the traditional pipeline approach using separate ASR → MT → TTS modules). This contrasts with direct S2ST by offering modularity and often higher quality in high-resource scenarios, but at the cost of error propagation, higher latency, and loss of prosody/speaker identity.

Direct S2ST (previous sections) bypasses text intermediates for better naturalness and efficiency, while cascaded approaches remain relevant baselines, especially when leveraging strong individual components or for prosody/expressive enhancements.

### Cascaded Speech-to-Speech Translation
- **[2406.00021] CrossVoice: Crosslingual Prosody Preserving Cascade-S2ST using Transfer Learning** (2024)  
  [https://arxiv.org/abs/2406.00021](https://arxiv.org/abs/2406.00021)  
  Novel cascade-based S2ST system with advanced ASR/MT/TTS + transfer learning for cross-lingual prosody preservation; compares favorably to direct methods on BLEU and MOS scores (e.g., Fisher Es-En, VoxPopuli Fr-En, CVSS-T).

- **[2301.10606] A Holistic Cascade System, benchmark, and Human Evaluation Protocol for Expressive Speech-to-Speech Translation** (2023)  
  [https://arxiv.org/abs/2301.10606](https://arxiv.org/abs/2301.10606)  
  Proposes a holistic cascaded expressive S2ST combining multiple prosody transfer techniques; includes benchmark and human evaluation protocol.

- **[2106.01045] Cascade versus Direct Speech Translation: Do the Differences Still Make a Difference?** (2021)  
  [https://arxiv.org/abs/2106.01045](https://arxiv.org/abs/2106.01045)  
  Systematic comparison of state-of-the-art cascaded vs. direct ST systems; analyzes if gaps persist in quality, latency, and other metrics.

- **[2502.00377] When End-to-End is Overkill: Rethinking Cascaded Speech-to-Text Translation** (2025)  
  [https://arxiv.org/abs/2502.00377](https://arxiv.org/abs/2502.00377)  
  Argues for cascaded models' continued relevance (despite error propagation criticism); explores multi-candidate ASR + self-supervised features for improved MT in cascaded pipelines (relevant to S2ST extensions).

### Foundational & Pioneering Papers (Direct S2ST)
- **[2107.05604] Direct speech-to-speech translation with discrete units** (2021)  
  [https://arxiv.org/abs/2107.05604](https://arxiv.org/abs/2107.05604)  
  Introduces direct S2ST predicting discrete speech units via self-supervised encoders + seq2seq.

- **[2107.08661] Translatotron 2: Robust direct speech-to-speech translation** (2021)  
  [https://arxiv.org/abs/2107.08661](https://arxiv.org/abs/2107.08661)  
  End-to-end model with strong voice preservation.

### Recent & Advanced Models (Direct S2ST, 2022–2026)
- **[2212.08055] UnitY: Two-pass Direct Speech-to-speech Translation with Discrete Units** (2022)  
  [https://arxiv.org/abs/2212.08055](https://arxiv.org/abs/2212.08055)  
  Two-pass for faster/better decoding.

- **[2308.11596] SeamlessM4T: Massively Multilingual & Multimodal Machine Translation** (2023)  
  [https://arxiv.org/abs/2308.11596](https://arxiv.org/abs/2308.11596)  
  Unified multilingual direct S2ST for ~100 languages.

- **[2312.05187] Seamless: Multilingual Expressive and Streaming Speech Translation** (2023)  
  [https://arxiv.org/abs/2312.05187](https://arxiv.org/abs/2312.05187)  
  Expressive prosody + streaming direct S2ST.

- **[2406.07289] Can We Achieve High-quality Direct Speech-to-Speech Translation without Parallel Speech Data?** (2024)  
  [https://arxiv.org/abs/2406.07289](https://arxiv.org/abs/2406.07289)  
  ComSpeech using pretrained S2TT + TTS.

- **[2412.07316] Preserving Speaker Information in Direct Speech-to-Speech Translation with Non-Autoregressive Generation and Pretraining** (2024)  
  [https://arxiv.org/abs/2412.07316](https://arxiv.org/abs/2412.07316)  
  Speaker preservation via non-autoregressive + pretraining.

- **[2601.16023] Timbre-Aware LLM-based Direct Speech-to-Speech Translation Extendable to Multiple Language Pairs** (2026)  
  [https://arxiv.org/abs/2601.16023](https://arxiv.org/abs/2601.16023)  
  LLM-based scalable direct S2ST preserving timbre.

### Surveys & Reviews (Covering Both Cascade and Direct)
- **[2503.04799] Direct Speech to Speech Translation: A Review** (2025)  
  [https://arxiv.org/abs/2503.04799](https://arxiv.org/abs/2503.04799)  
  Compares cascade (ASR/MT/TTS) vs. direct/end-to-end; discusses error propagation, latency, prosody loss in cascades.

- **[2411.14453] Direct Speech-to-Speech Neural Machine Translation: A Survey** (2024)  
  [https://arxiv.org/abs/2411.14453](https://arxiv.org/abs/2411.14453)  
  In-depth on direct S2ST architectures/metrics; notes historical dominance of cascades and ongoing gaps.

### Additional Notable Works (Direct S2ST)
- **[2203.13339] Leveraging unsupervised and weakly-supervised data to improve direct speech-to-speech translation** (2022)  
  [https://arxiv.org/abs/2203.13339](https://arxiv.org/abs/2203.13339)  
  Boosts direct S2ST with extra data; compares to cascade baselines.

- **[2305.17732] StyleS2ST: Zero-shot Style Transfer for Direct Speech-to-speech Translation** (2023)  
  [https://arxiv.org/abs/2305.17732](https://arxiv.org/abs/2305.17732)  
  Zero-shot style/prosody transfer in direct S2ST.

- **[2309.07566] Speech-to-Speech Translation with Discrete-Unit-Based Style Transfer** (2023)  
  [https://arxiv.org/abs/2309.07566](https://arxiv.org/abs/2309.07566)  
  Expressive direct output via discrete units + style transfer.

- **[2204.02967] Enhanced Direct Speech-to-Speech Translation Using Self-supervised Pre-training and Data Augmentation** (2022)  
  [https://arxiv.org/abs/2204.02967](https://arxiv.org/abs/2204.02967)  
  Addresses data scarcity in direct S2ST.



> To make this list even more comprehensive, feel free to share any additional papers you've come across (e.g., specific > > arXiv IDs, titles, or topics like low-resource African languages, expressive dubbing, or LLM-S2ST integrations). 
