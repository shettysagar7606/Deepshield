# DeepShield — System Architecture

## Layer 1 — Input
User provides video file via drag and drop 
desktop interface

## Layer 2 — USB Communication
Video frames streamed to AMD AI chip 
via USB 3.0 interface

## Layer 3 — AMD AI Processing
- AMD Ryzen AI NPU runs quantized EfficientNet model
- Frame level analysis for facial artifacts
- GAN pattern detection
- Audio visual sync check

## Layer 4 — Output
- REAL or DEEPFAKE verdict
- Confidence score percentage
- Flagged frame timestamps
- Optional PDF report export
