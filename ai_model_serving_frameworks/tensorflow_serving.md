# TensorFlow Serving

TensorFlow Serving is a flexible, high-performance serving system for machine learning models, designed for production environments. It deals with the inference aspect of machine learning, taking models after training and managing their lifetimes, providing clients with versioned access via a high-performance, reference-counted lookup table.

TensorFlow Serving provides out-of-the-box integration with TensorFlow models but can be easily extended to serve other types of models and data.

## Features

- Can serve multiple models, or multiple versions of the same model simultaneously
- Exposes both gRPC as well as HTTP inference endpoints
- Allows deployment of new model versions without changing any client code
- Supports canarying of new versions and A/B testing experimental models
- Adds minimal latency to inference time due to efficient, low-overhead implementation
- Features a scheduler that groups individual inference requests into batches for joint execution on GPU, with customizable policies to guide batching decisions

## Installation

TensorFlow Serving can be installed with Docker, apt-get, or by building from source. Detailed instructions can be found in the [official documentation](https://www.tensorflow.org/tfx/serving/setup).

## Usage

Once installed, you can start a serving server by pointing it to your model directory. Here's an example:

```bash
tensorflow_model_server --port=8501 --rest_api_port=8501 --model_name=my_model --model_base_path=/path/to/my_model/
```

This will start a server listening on port 8501 that you can send HTTP POST requests to for inference.

## Resources

- [Official Documentation](https://www.tensorflow.org/tfx/serving/serving_basic)
- [GitHub Repository](https://github.com/tensorflow/serving)
- [Docker Image](https://hub.docker.com/r/tensorflow/serving)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before getting started.

## Contact

If you have any questions, feel free to reach out to us. You can also raise an issue for any bugs/errors that you find in the project.

## Acknowledgements

We would like to thank all the contributors who have helped us in making this project better. Your contributions have been invaluable.
