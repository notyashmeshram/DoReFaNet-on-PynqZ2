# DoReFaNet on Pynq-Z2 Board

## Overview

This project demonstrates the implementation of **DoReFaNet**, a deep learning architecture optimized for image classification, deployed on the **Pynq-Z2 board** using the Xilinx **PYNQ** framework. By applying techniques like structured pruning and 8-bit quantization, the model achieves a smaller size and faster inference while maintaining a balance between accuracy and performance. The project further tunes data flow and memory usage to ensure FPGA compatibility and provides detailed evaluation of model performance, including accuracy, latency, and power consumption.

## Key Features
- **DoReFaNet Architecture**: Implemented a deep neural network tailored for efficient image classification.
- **Model Optimization**: 
  - Structured pruning to remove less important connections and reduce model size.
  - 8-bit quantization to enable faster computations and reduced power consumption without significant accuracy loss.
- **FPGA Deployment**: Deployed the optimized model on the Pynq-Z2 board, leveraging its FPGA capabilities to improve inference speed and efficiency.
- **Performance Evaluation**: Measured the model's performance based on accuracy, inference latency, and power consumption on the FPGA hardware.

## Hardware Setup

### Pynq-Z2 Board
This project is designed to run on the **Pynq-Z2 board**. Please ensure you are using the **v2.6 PYNQ image** for compatibility with the project files. You can download the PYNQ image from the official [TUL PYNQ-Z2 website](https://www.tulembedded.com/FPGA/ProductsPYNQ-Z2.html).

### PYNQ Framework
The Xilinx PYNQ framework provides an easy-to-use Python API for FPGA programming. For more information about PYNQ and the boards it supports, visit the official [PYNQ website](https://www.pynq.io/boards.html).

## Model Optimization Techniques

- **Structured Pruning**: Reduces the number of parameters in the neural network, decreasing both model size and computation requirements.
- **8-bit Quantization**: Converts model weights and activations to 8-bit representations, reducing memory usage and enabling faster computation on hardware without significant loss of accuracy.

## Performance Evaluation

The optimized model is evaluated based on the following metrics:
- **Accuracy**: Performance on the selected image classification dataset.
- **Latency**: Inference time for processing input images on the Pynq-Z2 board.
- **Power Consumption**: Monitored power usage during inference to assess the energy efficiency of the model on FPGA hardware.

## References

- [PYNQ Official Website](https://www.pynq.io/boards.html)
- [Pynq-Z2 Board Information and Downloads](https://www.tulembedded.com/FPGA/ProductsPYNQ-Z2.html)
