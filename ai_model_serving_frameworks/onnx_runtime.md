# ONNX Runtime

ONNX Runtime is a performance-focused engine for serving machine learning models, designed for production environments. It supports models in the Open Neural Network Exchange (ONNX) format which is an open standard for representing machine learning models. ONNX Runtime is designed to optimize and accelerate machine learning inference across a wide variety of machine learning frameworks, hardware, and operating systems.

## Features

- Can serve multiple models, or multiple versions of the same model simultaneously
- Exposes both gRPC as well as HTTP inference endpoints
- Allows deployment of new model versions without changing any client code
- Supports canarying of new versions and A/B testing experimental models
- Adds minimal latency to inference time due to efficient, low-overhead implementation
- Features a scheduler that groups individual inference requests into batches for joint execution on GPU, with customizable policies to guide batching decisions

## Installation

ONNX Runtime can be installed with pip, Docker, or by building from source. Detailed instructions can be found in the [official documentation](https://onnxruntime.ai/docs/build/).

## Usage

Once installed, you can start a serving server by pointing it to your model directory. Here's an example:

```bash
onnxruntime --model_path=/path/to/my_model.onnx
```

This will start a server that you can send HTTP POST requests to for inference.

## Resources

- [Official Documentation](https://onnxruntime.ai/docs/)
- [GitHub Repository](https://github.com/microsoft/onnxruntime)
- [Docker Image](https://hub.docker.com/r/onnxruntime/onnxruntime)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before getting started.

## Contact

If you have any questions, feel free to reach out to us. You can also raise an issue for any bugs/errors that you find in the project.

## Acknowledgements

We would like to thank all the contributors who have helped us in making this project better. Your contributions have been invaluable.
