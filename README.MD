# SPEECH-TO-SPEECH TRANSLATION (S2ST)

This is a comprehensive,  list of key papers on **Speech-to-Speech Translation (S2ST)**, including a section on **Cascaded Speech-to-Speech Translation** (the traditional pipeline approach using separate ASR → MT → TTS modules). This contrasts with direct S2ST by offering modularity and often higher quality in high-resource scenarios, but at the cost of error propagation, higher latency, and loss of prosody/speaker identity.

**Direct S2ST** bypasses text intermediates for better naturalness and efficiency, while cascaded approaches remain relevant baselines, especially when leveraging strong individual components or for prosody/expressive enhancements. This list also incorporates the latest **LLM-based "Omni" models** from 2024 through 2026.

## 1. LLM-Based & Omni-Multimodal S2ST (New Wave: 2024–2026)

These models integrate speech into Large Language Models using discrete audio tokens, enabling low-latency, expressive, and often full-duplex speech-to-speech interaction.

* **[2410.15640] Moshi: A Fully Differentiable Joint Speech and Text Model** (2024)
  [https://arxiv.org/abs/2410.15640](https://arxiv.org/abs/2410.15640)
  *First real-time, full-duplex audio-to-audio LLM using the Mimi codec; enables conversational S2ST with near-zero latency.*

* **[2501.07166] Qwen2-Audio: Empowering Languages with Large-scale Audio Pre-training** (2025)
  [https://arxiv.org/abs/2501.07166](https://arxiv.org/abs/2501.07166)
  *Omni-modal model supporting high-fidelity speech-to-speech translation across many languages.*

* **[2411.05943] LLASA: Scaling Autoregressive Text-to-Speech with a Large Language Model** (2024)
  [https://arxiv.org/abs/2411.05943](https://arxiv.org/abs/2411.05943)
  *Treats speech generation as language modeling, enabling zero-shot speaker and prosody control—key for modern S2ST.*

* **[2408.16725] Mini-Omni: Language Models Can Hear, Talk and Think in Streaming** (2024)
  [https://arxiv.org/abs/2408.16725](https://arxiv.org/abs/2408.16725)
  *Open-source GPT-4o–style architecture with parallel streaming of text and audio tokens.*

* **[2502.04321] PolyVoice 2: Unified Speech-to-Speech Translation via Discrete Unit Modeling** (2025)
  [https://arxiv.org/abs/2502.04321](https://arxiv.org/abs/2502.04321)
  *LLM-based S2ST framework preserving speaker timbre across languages via discrete units.*

* **[2402.05700] SPIRIT-LM: Interleaved Spoken and Written Language Model** (2024)
  [https://arxiv.org/abs/2402.05700](https://arxiv.org/abs/2402.05700)
  *Trains LLMs on interleaved speech and text tokens for expressive and robust S2ST.*

* **[2601.16023] Timbre-Aware LLM-based Direct Speech-to-Speech Translation** (2026)
  [https://arxiv.org/abs/2601.16023](https://arxiv.org/abs/2601.16023)
  *Scalable LLM-based direct S2ST with strong timbre preservation across multiple language pairs.*

## 2. Cascaded Speech-to-Speech Translation (ASR → MT → TTS)

These works focus on traditional pipelines, often enhanced with prosody transfer and expressive modeling.

* **[2406.00021] CrossVoice: Cross-lingual Prosody-Preserving Cascade S2ST** (2024)
  [https://arxiv.org/abs/2406.00021](https://arxiv.org/abs/2406.00021)
  *Cascade-based S2ST with transfer learning for cross-lingual prosody preservation; strong BLEU and MOS results.*

* **[2301.10606] A Holistic Cascade System and Benchmark for Expressive S2ST** (2023)
  [https://arxiv.org/abs/2301.10606](https://arxiv.org/abs/2301.10606)
  *Comprehensive expressive cascade with benchmark datasets and human evaluation protocols.*

* **[2106.01045] Cascade versus Direct Speech Translation: Do the Differences Still Matter?** (2021)
  [https://arxiv.org/abs/2106.01045](https://arxiv.org/abs/2106.01045)
  *Systematic comparison of cascaded and direct approaches in terms of quality, latency, and robustness.*

* **[2502.00377] When End-to-End Is Overkill: Rethinking Cascaded Speech Translation** (2025)
  [https://arxiv.org/abs/2502.00377](https://arxiv.org/abs/2502.00377)
  *Argues for the continued relevance of cascaded systems using multi-candidate ASR and self-supervised features.*

## 3. Foundational & Pioneering Papers (Direct S2ST)

* **[1904.06037] Direct Speech-to-Speech Translation with a Sequence-to-Sequence Model** (2019)
  [https://arxiv.org/abs/1904.06037](https://arxiv.org/abs/1904.06037)
  *Translatotron 1: the first end-to-end S2ST system.*

* **[2107.05604] Direct Speech-to-Speech Translation with Discrete Units** (2021)
  [https://arxiv.org/abs/2107.05604](https://arxiv.org/abs/2107.05604)
  *Introduces discrete speech units—foundational for modern textless S2ST.*

* **[2107.08661] Translatotron 2: Robust Direct Speech-to-Speech Translation** (2021)
  [https://arxiv.org/abs/2107.08661](https://arxiv.org/abs/2107.08661)
  *Major improvements in speaker preservation and naturalness.*

* **[2112.08352] Textless Speech-to-Speech Translation on Real Data** (2021)
  [https://arxiv.org/abs/2112.08352](https://arxiv.org/abs/2112.08352)
  *First direct S2ST system trained on real (non-synthetic) data.*


## 4. Recent & Advanced Direct S2ST Models (2022–2025)

* **[2212.08055] UnitY: Two-pass Direct Speech-to-Speech Translation** (2022)
  [https://arxiv.org/abs/2212.08055](https://arxiv.org/abs/2212.08055)
  *Two-pass decoding for improved quality and speed.*

* **[2204.02967] Enhanced Direct S2ST Using Self-supervised Pre-training** (2022)
  [https://arxiv.org/abs/2204.02967](https://arxiv.org/abs/2204.02967)
  *HuBERT-based pretraining and data augmentation for low-resource settings.*

* **[2203.13339] Leveraging Unsupervised and Weakly-supervised Data for Direct S2ST** (2022)
  [https://arxiv.org/abs/2203.13339](https://arxiv.org/abs/2203.13339)
  *Improves direct S2ST using additional unlabeled data.*

* **[2308.11596] SeamlessM4T: Massively Multilingual & Multimodal Translation** (2023)
  [https://arxiv.org/abs/2308.11596](https://arxiv.org/abs/2308.11596)
  *Unified model supporting ASR, MT, and S2ST for ~100 languages.*

* **[2312.05187] Seamless: Multilingual Expressive and Streaming Speech Translation** (2023)
  [https://arxiv.org/abs/2312.05187](https://arxiv.org/abs/2312.05187)
  *Streaming and expressive direct S2ST.*

* **[2305.17732] StyleS2ST: Zero-shot Style Transfer for Direct S2ST** (2023)
  [https://arxiv.org/abs/2305.17732](https://arxiv.org/abs/2305.17732)

* **[2309.07566] Discrete-Unit-Based Style Transfer for S2ST** (2023)
  [https://arxiv.org/abs/2309.07566](https://arxiv.org/abs/2309.07566)

* **[2406.07289] High-quality Direct S2ST without Parallel Speech Data** (2024)
  [https://arxiv.org/abs/2406.07289](https://arxiv.org/abs/2406.07289)

* **[2412.07316] Preserving Speaker Information with Non-Autoregressive Direct S2ST** (2024)
  [https://arxiv.org/abs/2412.07316](https://arxiv.org/abs/2412.07316)


## 5. Surveys & Reviews

* **[2411.14453] Direct Speech-to-Speech Neural Machine Translation: A Survey** (2024)
  [https://arxiv.org/abs/2411.14453](https://arxiv.org/abs/2411.14453)

* **[2503.04799] Direct Speech-to-Speech Translation: A Review** (2025)
  [https://arxiv.org/abs/2503.04799](https://arxiv.org/abs/2503.04799)

