# Native Libraries Collection

A curated collection of **112 native Android libraries** (ARM64/aarch64) organized into functional categories. These libraries cover machine learning inference, React Native framework components, image processing, speech synthesis, hardware acceleration, and more.

## Repository Structure

| Category | Libraries | Description |
|----------|-----------|-------------|
| [ml-inference](./ml-inference/) | 22 | Machine learning and AI inference engines |
| [react-native](./react-native/) | 35 | React Native framework and Hermes engine |
| [image-processing](./image-processing/) | 8 | Image manipulation and computer vision |
| [speech-audio](./speech-audio/) | 5 | Speech synthesis and audio processing |
| [nlp-text](./nlp-text/) | 5 | Natural language processing and tokenization |
| [hardware-acceleration](./hardware-acceleration/) | 9 | GPU, NPU, and hardware optimization |
| [crash-monitoring](./crash-monitoring/) | 5 | Crash reporting and error tracking |
| [storage-data](./storage-data/) | 3 | Key-value storage and data persistence |
| [ui-animation](./ui-animation/) | 5 | UI layout and animation engines |
| [networking-ads](./networking-ads/) | 3 | Advertising SDKs and networking |
| [utilities](./utilities/) | 6 | Compression, admin tools, and utilities |
| [runtime-core](./runtime-core/) | 6 | C++ runtime and logging frameworks |

## Categories

### ml-inference

Machine learning inference libraries including TensorFlow Lite, ONNX Runtime, llama.cpp, GGML, and MediaPipe.

- `libtensorflowlite_jni_stable.so` - TensorFlow Lite inference engine
- `libonnxruntime.so` - ONNX Runtime inference engine
- `libonnxruntime4j_jni.so` - ONNX Runtime Java bindings
- `libonnxruntimejsihelper.so` - ONNX Runtime JSI helper
- `libllama.so` - llama.cpp LLM inference
- `libllama-jni.so` - llama.cpp Java bindings
- `libexecutorch_llama_jni.so` - ExecuTorch Llama inference
- `libncnn.so` - NCNN neural network inference
- `libggml.so` - GGML tensor library
- `libggml-base.so` - GGML base library
- `libggml-blas.so` - GGML BLAS backend
- `libggml-cpu.so` - GGML CPU backend
- `libggml-opencl.so` - GGML OpenCL backend
- `libggml-vulkan.so` - GGML Vulkan backend
- `libtvm4j_runtime_packed.so` - Apache TVM runtime
- `libmediapipe_tasks_vision_image_generator_jni.so` - MediaPipe image generation
- `libctranslate2.so` - CTranslate2 inference engine
- `libctranslate2-jni.so` - CTranslate2 Java bindings
- `libsherpa-onnx-jni.so` - Sherpa ONNX speech recognition
- `libsd-jni.so` - Stable Diffusion JNI
- `liblaylaQNN.so` - Qualcomm QNN integration
- `libaiai_native.so` - Google AI services

### react-native

React Native framework components including Hermes JavaScript engine, Fabric renderer, and Expo modules.

- `libreact_codegen_rncore.so` - React Native codegen
- `libreact_cxxreactpackage.so` - React Native C++ package
- `libreact_debug.so` - React Native debug utilities
- `libreact_devsupportjni.so` - React Native dev support
- `libreact_featureflags.so` - React Native feature flags
- `libreact_featureflagsjni.so` - Feature flags JNI
- `libreact_nativemodule_core.so` - Native module core
- `libreact_newarchdefaults.so` - New architecture defaults
- `libreact_render_componentregistry.so` - Component registry
- `libreact_render_core.so` - Render core
- `libreact_render_debug.so` - Render debug
- `libreact_render_graphics.so` - Render graphics
- `libreact_render_imagemanager.so` - Image manager
- `libreact_render_mapbuffer.so` - Map buffer
- `libreact_utils.so` - React Native utilities
- `libreactnativeblob.so` - Blob handling
- `libreactnativejni.so` - React Native JNI
- `libreactperfloggerjni.so` - Performance logger
- `librninstance.so` - RN instance
- `librnscreens.so` - React Navigation screens
- `librrc_image.so` - Image component
- `librrc_legacyviewmanagerinterop.so` - Legacy view manager
- `librrc_view.so` - View component
- `libturbomodulejsijni.so` - TurboModules JSI
- `libfabricjni.so` - Fabric renderer JNI
- `libfbjni.so` - Facebook JNI utilities
- `libhermes.so` - Hermes JavaScript engine
- `libhermes_executor.so` - Hermes executor
- `libhermesinstancejni.so` - Hermes instance JNI
- `libjscinstance.so` - JavaScriptCore instance
- `libjsi.so` - JavaScript Interface
- `libjsijniprofiler.so` - JSI JNI profiler
- `libjsinspector.so` - JS inspector
- `libexpo-modules-core.so` - Expo modules core
- `libmapbufferjni.so` - Map buffer JNI

### image-processing

Image manipulation, filtering, and computer vision libraries.

- `libimage_processing_util_jni.so` - Image processing utilities
- `libimagegenerator_gpu.so` - GPU image generation
- `libimagepipeline.so` - Fresco image pipeline
- `libnative-filters.so` - Native image filters
- `libnative-imagetranscoder.so` - Image transcoding
- `libim2intent_jni.so` - Image to intent
- `libbarhopper_v2.so` - Barcode/QR scanning
- `libparticle-extractor_jni.so` - Particle extraction

### speech-audio

Speech synthesis, recognition, and audio processing libraries.

- `libespeak-ng.so` - eSpeak NG text-to-speech
- `libpiper_phonemize.so` - Piper phonemization
- `libkaldi-decoder-core.so` - Kaldi speech decoder
- `libkaldi-native-fbank-core.so` - Kaldi filterbank
- `libdps_soda_jni.so` - Google speech recognition

### nlp-text

Natural language processing, text classification, and tokenization.

- `libtextclassifier3_jni_aiai.so` - Text classification
- `libsentencepiece.so` - SentencePiece tokenizer
- `libsentencepiece_train.so` - SentencePiece training
- `libssentencepiece_core.so` - SentencePiece core
- `libtokenizers-jni.so` - HuggingFace tokenizers

### hardware-acceleration

Hardware acceleration libraries for GPU, NPU, and optimized compute.

- `libQnnHtpV68Stub.so` - Qualcomm HTP v68
- `libQnnHtpV69Stub.so` - Qualcomm HTP v69
- `libQnnHtpV73Stub.so` - Qualcomm HTP v73
- `libQnnHtpV75Stub.so` - Qualcomm HTP v75
- `libQnnHtpV79Stub.so` - Qualcomm HTP v79
- `libOpenCL.so` - OpenCL compute
- `libopenblas.so` - OpenBLAS linear algebra
- `libomp.so` - OpenMP threading
- `libcpuutils.so` - CPU utilities

### crash-monitoring

Crash reporting and error monitoring libraries.

- `libcrashlytics.so` - Firebase Crashlytics
- `libcrashlytics-common.so` - Crashlytics common
- `libcrashlytics-handler.so` - Crashlytics handler
- `libcrashlytics-trampoline.so` - Crashlytics trampoline
- `libapplovin-native-crash-reporter.so` - AppLovin crash reporter

### storage-data

Key-value storage and data persistence libraries.

- `libmmkv.so` - MMKV key-value storage
- `liblvdb-jni.so` - LevelDB JNI
- `libmappedcountercacheversionjni.so` - Mapped counter cache

### ui-animation

UI layout engines and animation libraries.

- `libreanimated.so` - React Native Reanimated
- `librive-android.so` - Rive animation runtime
- `libyoga.so` - Yoga layout engine
- `libuimanagerjni.so` - UI manager JNI
- `libsurface_util_jni.so` - Surface utilities

### networking-ads

Advertising SDKs and networking libraries.

- `libgluads_shared.so` - Glu ads SDK
- `libtapjoy.so` - Tapjoy ads SDK
- `libclient_android_jni.so` - Client networking

### utilities

Compression, administration, and utility libraries.

- `libNimble.so` - Nimble utilities
- `libtcmadmin.so` - TC admin
- `libtcmadmin21.so` - TC admin v21
- `libtcnative.so` - TC native
- `libtcun7zip.so` - 7-Zip compression
- `libucd.so` - Unicode data

### runtime-core

C++ runtime libraries, logging, and core dependencies.

- `libc++_shared.so` - LLVM C++ standard library
- `libfolly_runtime.so` - Facebook Folly runtime
- `libruntimeexecutor.so` - Runtime executor
- `libglog.so` - Google logging
- `libspdlog.so` - Fast C++ logging
- `libapprunner.so` - App runner

## Architecture

All libraries in this collection are compiled for **ARM64 (aarch64)** architecture, targeting Android devices.

## License

The libraries in this collection are subject to their respective licenses. Please refer to the original projects for licensing information.

## Contributing

Contributions are welcome! Please feel free to submit pull requests to add new libraries or improve categorization.
