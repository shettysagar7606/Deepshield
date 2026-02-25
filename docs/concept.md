# DeepShield — Concept Document

## Problem Statement
Deepfake videos are being weaponized for financial fraud, 
identity theft, political misinformation, and fabrication 
of evidence. Existing detection tools require users to 
upload sensitive videos to third-party cloud servers, 
creating a critical privacy risk. There is no offline, 
portable, and accessible solution that common users can 
use to instantly verify the authenticity of a video.

## Proposed Solution
DeepShield is a portable USB dongle powered by AMD's 
Ryzen AI chip. The entire deepfake detection model runs 
locally on the AMD NPU inside the dongle. Users simply 
plug it into any laptop and get instant results.

## Why AMD
AMD Ryzen AI chips contain a dedicated Neural Processing 
Unit (NPU) specifically designed for AI inference tasks. 
DeepShield leverages this NPU to run EfficientNet-B4 
deepfake detection model locally — fast, efficient, 
and without any cloud dependency.

## Dual Mode Operation
- AMD Device Mode: Natively runs on AMD Ryzen AI 
  powered laptops using the inbuilt NPU
- Universal Mode: USB dongle works on any 
  Windows or Mac system

## Detection Technology
- Model: EfficientNet-B4 fine-tuned on FaceForensics++
- Analyzes facial inconsistencies frame by frame
- Detects blinking pattern anomalies
- Identifies GAN fingerprints
- Checks audio-visual lip sync mismatch
- Returns confidence score with flagged timestamps
