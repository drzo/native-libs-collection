# Native Android Libraries Collection

A curated collection of high-quality native Android libraries (ARM64-v8a) organized by category. This repository contains **132 libraries** across **18 categories** for Android development.

## Repository Structure

| Category | Count | Description |
|----------|-------|-------------|
| [ml-inference](./ml-inference/) | 22 | TensorFlow Lite, ONNX Runtime, llama.cpp, GGML, MediaPipe, ncnn |
| [ml-inference-alibaba](./ml-inference-alibaba/) | 8 | **NEW** Alibaba MNN framework - blazing fast, lightweight DL |
| [react-native](./react-native/) | 35 | React Native framework, Hermes engine, Fabric, Expo |
| [image-processing](./image-processing/) | 14 | Image filters, barcode scanning, GPU generation, OpenCV-mobile |
| [speech-audio](./speech-audio/) | 5 | eSpeak, Kaldi, Piper phonemization |
| [speech-whisper](./speech-whisper/) | 4 | **NEW** Sherpa-ONNX for Whisper ASR and speech recognition |
| [nlp-text](./nlp-text/) | 5 | SentencePiece, HuggingFace tokenizers, text classification |
| [hardware-acceleration](./hardware-acceleration/) | 9 | Qualcomm QNN (HTP v68-v79), OpenCL, OpenBLAS |
| [crash-monitoring](./crash-monitoring/) | 5 | Firebase Crashlytics, AppLovin crash reporter |
| [storage-data](./storage-data/) | 3 | MMKV, LevelDB |
| [ui-animation](./ui-animation/) | 5 | Reanimated, Rive, Yoga layout |
| [networking-ads](./networking-ads/) | 3 | Tapjoy, Glu ads |
| [utilities](./utilities/) | 6 | 7-Zip, Unicode data, admin tools |
| [runtime-core](./runtime-core/) | 6 | libc++, Folly, glog, spdlog |
| [compression](./compression/) | 1 | **NEW** Facebook Zstd fast compression |
| [crypto-security](./crypto-security/) | 1 | **NEW** Libsodium modern encryption library |
| [media-processing](./media-processing/) | 0 | Reserved for FFmpeg, audio/video codecs |
| [communication](./communication/) | 0 | Reserved for WebRTC, gRPC |

## Newly Added Libraries (v2.0)

### MNN (Alibaba) - 13.8k GitHub Stars
Blazing fast, lightweight deep learning framework from Alibaba. Battle-tested in production with Android .so size of only ~800KB.

**Libraries included:**
- `libMNN.so` - Core inference engine
- `libMNN_CL.so` - OpenCL backend
- `libMNN_Vulkan.so` - Vulkan backend
- `libMNN_Express.so` - High-level API
- `libMNNOpenCV.so` - OpenCV compatibility layer
- `libllm.so` - LLM support
- `libmnncore.so` - Core utilities

### Sherpa-ONNX - 9.5k GitHub Stars
High-performance speech recognition supporting Whisper, SenseVoice, and many other ASR models.

**Libraries included:**
- `libsherpa-onnx-jni.so` - JNI bindings
- `libsherpa-onnx-c-api.so` - C API
- `libsherpa-onnx-cxx-api.so` - C++ API
- `libonnxruntime.so` - ONNX Runtime

### OpenCV-Mobile - 3.1k GitHub Stars
Minimal OpenCV build (~10x smaller than official SDK) for Android.

**Libraries included (static):**
- `libopencv_core.a`
- `libopencv_imgproc.a`
- `libopencv_highgui.a`
- `libopencv_features2d.a`
- `libopencv_photo.a`
- `libopencv_video.a`

### Zstd (Facebook) - Fast Compression
Facebook's fast lossless compression algorithm with JNI bindings.

**Libraries included:**
- `libzstd-jni-1.5.6-8.so`

### Libsodium - Modern Cryptography
Modern, portable, easy-to-use crypto library for encryption, signatures, and password hashing.

**Libraries included:**
- `libsodium.so`

## Category Details

### ml-inference
Core machine learning inference engines for running models on-device:
- **TensorFlow Lite** - Google's lightweight ML framework
- **ONNX Runtime** - Cross-platform ML inference
- **llama.cpp / GGML** - Efficient LLM inference
- **ncnn** - Tencent's high-performance neural network inference
- **MediaPipe** - Google's ML solutions for live and streaming media
- **ExecuTorch** - Meta's on-device AI framework
- **CTranslate2** - Fast inference engine for Transformer models

### hardware-acceleration
Libraries for leveraging device-specific hardware:
- **Qualcomm QNN** - Neural Processing Unit acceleration (HTP v68-v79)
- **OpenCL** - GPU compute
- **OpenBLAS** - Optimized BLAS library
- **Vulkan** - Low-overhead graphics and compute

### react-native
Complete React Native ecosystem:
- **Hermes** - JavaScript engine optimized for React Native
- **Fabric** - New rendering system
- **Reanimated** - Smooth animations
- **Expo** - Development platform

## Architecture

All libraries are compiled for **ARM64-v8a** (64-bit ARM) architecture, which is the standard for modern Android devices.

## Usage

1. Clone this repository
2. Copy the required `.so` files to your project's `jniLibs/arm64-v8a/` directory
3. Load the libraries in your code using `System.loadLibrary()`

```java
static {
    System.loadLibrary("MNN");
    System.loadLibrary("MNN_CL");
}
```

## License

Each library retains its original license. Please refer to the respective project repositories for licensing information.

## Contributing

Contributions are welcome! Please submit a pull request with:
1. The compiled `.so` file(s)
2. Source repository link
3. License information
4. Brief description of the library's purpose

## Changelog

### v2.0 (December 2025)
- Added MNN (Alibaba) ML inference framework
- Added Sherpa-ONNX for Whisper/ASR support
- Added OpenCV-mobile minimal computer vision library
- Added Zstd compression library
- Added Libsodium cryptography library
- New categories: compression, crypto-security, media-processing, communication
- Total libraries: 132

### v1.0 (December 2025)
- Initial release with 112 libraries across 12 categories
