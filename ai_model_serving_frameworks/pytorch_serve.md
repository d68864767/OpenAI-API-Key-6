# PyTorch Serve

PyTorch Serve is a flexible, high-performance serving system for machine learning models, designed for production environments. It is part of the PyTorch project and is primarily used to serve PyTorch models but can be extended to serve other model types.

## Features

- Can serve multiple models, or multiple versions of the same model simultaneously
- Exposes both gRPC as well as HTTP inference endpoints
- Allows deployment of new model versions without changing any client code
- Supports canarying of new versions and A/B testing experimental models
- Adds minimal latency to inference time due to efficient, low-overhead implementation
- Features a scheduler that groups individual inference requests into batches for joint execution on GPU, with customizable policies to guide batching decisions

## Installation

PyTorch Serve can be installed with pip, Docker, or by building from source. Detailed instructions can be found in the [official documentation](https://pytorch.org/serve/).

## Usage

Once installed, you can start a serving server by pointing it to your model directory. Here's an example:

```bash
torchserve --start --ncs --model-store /path/to/my_model/ --models my_model=my_model.pt
```

This will start a server that you can send HTTP POST requests to for inference.

## Resources

- [Official Documentation](https://pytorch.org/serve/)
- [GitHub Repository](https://github.com/pytorch/serve)
- [Docker Image](https://hub.docker.com/r/pytorch/pytorch)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before getting started.

## Contact

If you have any questions, feel free to reach out to us. You can also raise an issue for any bugs/errors that you find in the project.

## Acknowledgements

We would like to thank all the contributors who have helped us in making this project better. Your contributions have been invaluable.
