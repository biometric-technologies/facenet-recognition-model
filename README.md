![](.github/readme/banner.svg)

# FaceNet recognition model

This repository is reserved for the FaceNet face embedding model of the Iriscan face pipeline. It is empty for now: no code, weights or releases have been published here yet.

FaceNet is a neural network that turns a cropped face image into an embedding, a fixed-length list of numbers, such that two photos of the same person give embeddings that lie close together and photos of different people lie far apart, so comparing faces becomes measuring a distance.

The [Biometric SDK](https://github.com/biometric-technologies/biometric-sdk) runs a FaceNet-type model as a TensorFlow Lite file that you supply through `FaceNetModelConfiguration(path, inputWidth, inputHeight, outputLength)`; [tensorflow-facenet-model-test](https://github.com/biometric-technologies/tensorflow-facenet-model-test) is a script for checking such a `.tflite` model on your own photos. To run the model outside TensorFlow Lite, see [biometric-models-onnx-converters](https://github.com/biometric-technologies/biometric-models-onnx-converters), which exports FaceNet from facenet-pytorch to ONNX.

License: not yet specified. Contact: info@iriscan.com, https://www.iriscan.com
