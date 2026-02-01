# THE COMPREHENSIVE TTS READING LIST (2016–2026)

### End-to-End Autoregressive Foundations
Before this, TTS relied on HMMs or unit selection. These papers proved that neural networks could map text directly to audio features.

*   **[1609.03499] WaveNet: A Generative Model for Raw Audio** (2016)  
    [https://arxiv.org/abs/1609.03499](https://arxiv.org/abs/1609.03499)  
    *The revolution in high-fidelity audio. It used dilated causal convolutions to generate raw audio samples.*
*   **[1703.10135] Tacotron: Towards End-to-End Speech Synthesis** (2017)  
    [https://arxiv.org/abs/1703.10135](https://arxiv.org/abs/1703.10135)  
    *The foundational Seq2Seq TTS paper using an encoder-decoder with attention.*
*   **[1712.05884] Tacotron 2: Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrograms** (2017)  
    [https://arxiv.org/abs/1712.05884](https://arxiv.org/abs/1712.05884)  
    *The industry-standard architecture for years: simplified Tacotron 1 + Mel-spectrogram prediction + WaveNet vocoder.*


### Non-Autoregressive Speed & Robustness
Autoregressive models were slow and unstable. These papers solved word-skipping and inference speed issues.

*   **[1905.09263] FastSpeech: Fast, Robust and Controllable Text to Speech** (2019)  
    [https://arxiv.org/abs/1905.09263](https://arxiv.org/abs/1905.09263)  
    *Introduced the "Length Regulator" to allow parallel (non-autoregressive) speech synthesis.*
*   **[2006.04558] FastSpeech 2: Fast and High-Quality End-to-End TTS** (2020)  
    [https://arxiv.org/abs/2006.04558](https://arxiv.org/abs/2006.04558)  
    *Added explicit variance predictors (pitch, energy, duration), making the model much easier to train.*
*   **[2005.11129] Glow-TTS: A Generative Flow-based Model for High-quality TTS** (2020)  
    [https://arxiv.org/abs/2005.11129](https://arxiv.org/abs/2005.11129)  
    *Used Normalizing Flows to learn the alignment between text and speech internally.*


### Unified End-to-End Synthesis (The VITS Era)
This phase bridged the gap between acoustic modeling and waveform generation.

*   **[2106.00038] VITS: Conditional Variational Autoencoder with Adversarial Learning for E2E TTS** (2021) ⭐  
    [https://arxiv.org/abs/2106.00038](https://arxiv.org/abs/2106.00038)  
    *The bridge: It unified alignment, acoustic modeling, and vocoding into one model using flows and GANs. It is still a very popular baseline today.*
*   **[2010.05646] HiFi-GAN: Generative Adversarial Networks for Efficient Speech Synthesis** (2020)  
    [https://arxiv.org/abs/2010.05646](https://arxiv.org/abs/2010.05646)  
    *The standard neural vocoder that achieved human-level fidelity with extreme inference speed.*


### Diffusion & Flow-Matching TTS
Following the success of DALL-E 2, TTS research adopted diffusion to model the complex distribution of speech.

*   **[2105.06337] Grad-TTS: A Diffusion Probabilistic Model for Text-to-Speech** (2021)  
    [https://arxiv.org/abs/2105.06337](https://arxiv.org/abs/2105.06337)  
    *Pioneered score-based diffusion for speech generation.*
*   **[2304.09116] NaturalSpeech 2: Latent Diffusion Models are Zero-Shot TTS Synthesizers** (2023)  
    [https://arxiv.org/abs/2304.09116](https://arxiv.org/abs/2304.09116)  
    *Used latent diffusion to achieve high-quality zero-shot cloning with very short prompts.*
*   **[2409.02877] F5-TTS: A Simple and Strong Zero-shot TTS System via Diffusion Transformer** (2024)  
    [https://arxiv.org/abs/2409.02877](https://arxiv.org/abs/2409.02877)  
    *Latest state-of-the-art in Flow-Matching (a faster alternative to Diffusion) using a Transformer backbone.*


### Neural Audio Codecs & Codec Language Models (The VALL-E Era)
This is the "Representation Learning" of TTS. Instead of spectrograms, we now predict discrete audio tokens.

*   **[1711.00937] Neural Discrete Representation Learning (VQ-VAE)** (2017)  
    [https://arxiv.org/abs/1711.00937](https://arxiv.org/abs/1711.00937)  
    *The "Grandfather" paper. It introduced the Vector Quantization used in modern audio codecs.*
*   **[2210.13438] High-Fidelity Audio Compression with EnCodec** (2022)  
    [https://arxiv.org/abs/2210.13438](https://arxiv.org/abs/2210.13438)  
    *The neural codec that turned audio into "discrete tokens" for LLMs to read.*
*   **[2301.02111] VALL-E: Neural Codec Language Models are Zero-Shot TTS Synthesizers** (2023)  
    [https://arxiv.org/abs/2301.02111](https://arxiv.org/abs/2301.02111)  
    *The breakthrough: Treated TTS as a "language modeling continuation" task. Started the current trend of prompting for voice cloning.*


### Modern Generative Speech-LLMs (2024–2026)
The current frontier: Unified architectures, scaling compute, and continuous autoregressive modeling.

*   **[2407.08551] Autoregressive Speech Synthesis without Vector Quantization (MELLE)** (2024)  
    [https://arxiv.org/abs/2407.08551](https://arxiv.org/abs/2407.08551)  
    *Proves that autoregressive TTS can work without discrete tokens, using continuous values to avoid robotic artifacts.*
*   **[2411.05943] LLASA: Scaling Autoregressive Text-to-Speech with A LLM** (2024)  
    [https://arxiv.org/abs/2411.05943](https://arxiv.org/abs/2411.05943)  
    *Explores the scaling laws of speech synthesis when using a large LLM backbone.*
*   **[2410.15640] Moshi: a Fully Differentiable Joint Speech and Text Model** (2024/2025)  
    [https://arxiv.org/abs/2410.15640](https://arxiv.org/abs/2410.15640)  
    *The first full-duplex conversational model. Its TTS is generated in parallel with text for zero-latency.*
*   **[2502.04321] PolyVoice 2: Unified Speech Generation via Discrete Unit Modeling** (2025)  
    [https://arxiv.org/abs/2502.04321](https://arxiv.org/abs/2502.04321)  
    *The absolute latest in unified generation, focusing on extreme prosody control and multi-speaker consistency.*


### Evaluation & Surveys
*   **[2306.12424] A Survey on Neural Speech Synthesis** (2023)  
    [https://arxiv.org/abs/2306.12424](https://arxiv.org/abs/2306.12424)  
    *The most comprehensive modern review of the field.*
*   **[2410.03058] Large Language Models for Speech Processing: A Survey** (2024)  
    [https://arxiv.org/abs/2410.03058](https://arxiv.org/abs/2410.03058)  
    *Explains the transition from Phase 1-4 models to the current Phase 5-6 LLM models.*