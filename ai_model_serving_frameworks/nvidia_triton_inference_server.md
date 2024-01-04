# Nvidia Triton Inference Server

Nvidia Triton Inference Server is a flexible, high-performance serving system for machine learning models, designed for production environments. It supports a wide range of machine learning frameworks, including TensorFlow, PyTorch, ONNX, and others. Triton Inference Server is designed to optimize and accelerate machine learning inference in both cloud and edge environments.

## Features

- Can serve multiple models, or multiple versions of the same model simultaneously
- Exposes both gRPC as well as HTTP inference endpoints
- Allows deployment of new model versions without changing any client code
- Supports canarying of new versions and A/B testing experimental models
- Adds minimal latency to inference time due to efficient, low-overhead implementation
- Features a scheduler that groups individual inference requests into batches for joint execution on GPU, with customizable policies to guide batching decisions

## Installation

Nvidia Triton Inference Server can be installed with Docker, or by building from source. Detailed instructions can be found in the [official documentation](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/quickstart.html).

## Usage

Once installed, you can start a serving server by pointing it to your model directory. Here's an example:

```bash
tritonserver --model-repository=/path/to/my_model/
```

This will start a server that you can send HTTP POST requests to for inference.

## Resources

- [Official Documentation](https://docs.nvidia.com/deeplearning/triton-inference-server/user-guide/docs/)
- [GitHub Repository](https://github.com/triton-inference-server/server)
- [Docker Image](https://hub.docker.com/r/nvcr.io/nvidia/tritonserver)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before getting started.

## Contact

If you have any questions, feel free to reach out to us. You can also raise an issue for any bugs/errors that you find in the project.

## Acknowledgements

We would like to thank the Nvidia team for creating and maintaining the Triton Inference Server project.
