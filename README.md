🎵 Audio Generation Using Generative AI (MUSICGEN)
📘 Project Overview

Audio Generation Using Generative AI explores the use of deep learning for generating realistic, high-quality music from text and melody inputs.
This project implements MUSICGEN, a single-stage Transformer-based model that eliminates multi-stage hierarchies and enables controllable text-to-music and melody-conditioned music generation.

🎯 Objectives

Build a simple yet controllable music generation model using Generative AI.

Leverage Transformer architectures for efficient sequence modeling.

Incorporate text and melody conditioning for creative control.

Evaluate the system using objective and human-based audio quality metrics.

🧠 Key Features

🎶 Text-to-Music Generation: Generates music from descriptive text prompts.

🎧 Melody Conditioning: Produces music that follows a given melody or tune.

⚡ Single-Stage Transformer: Simplifies model design using token interleaving patterns.

🔊 High-Quality Output: Generates realistic, coherent, and stereo audio at 32 kHz.

🧩 Evaluation Metrics: Uses Fréchet Audio Distance (FAD), KL Divergence, CLAP score, and Human Mean Opinion Score (MOS).

🧱 System Architecture

Audio Tokenization (EnCodec + RVQ)

Converts raw audio into discrete token sequences for efficient modeling.

Codebook Interleaving Patterns

Delay, Parallel, Flattening, and Coarse-first methods to balance quality and computation.

Model Conditioning

Text conditioning using T5 / CLAP encoders.

Melody conditioning using chromagram-based representations.

Autoregressive Transformer Decoder

Generates audio token sequences step-by-step based on conditioning input.

⚙️ Technologies Used

Python

PyTorch / Transformers

Generative AI Models (VAE, GAN, Transformer)

Audio Processing (Librosa, EnCodec)

NumPy, Matplotlib, Scipy

📊 Evaluation
Metric	Description	Result
FAD (↓)	Measures audio realism	3.4
CLAP Score (↑)	Audio-text alignment	0.32
Human Rating (↑)	Perceived quality	84.8 / 100
Dataset	Licensed 20K-hour music dataset	—
📈 Results Summary

MUSICGEN outperformed baselines such as Riffusion, Mousai, and MusicLM.

Achieved high-quality stereo generation with efficient training.

Demonstrated better text and melody adherence compared to prior multi-stage methods.



📚 References

Jade Copet et al., “Simple and Controllable Music Generation (MUSICGEN)”, NeurIPS 2023.

A. Agostinelli et al., “MusicLM: Generating Music from Text”, Google Research, 2023.

Alexandre Défossez et al., “High Fidelity Neural Audio Compression (EnCodec)”, Meta AI, 2022.
