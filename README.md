Assignment Solutions: Edge AI, Quantum AI, and IoT Implementation

This repository contains the complete solution set for the Theoretical Analysis and Practical Implementation assignments. The solutions are divided into four files, covering theoretical essays, a working Python prototype, and system design documentation.

File Structure

File Name

Description

theoretical_analysis.md

Part 1: Essays on Edge AI latency/privacy and Quantum AI optimization.

edge_ai_prototype.py

Part 2 (Task 1): Python script to train a lightweight CNN and convert it to TensorFlow Lite.

edge_ai_report.md

Part 2 (Task 1): Report detailing the prototype's accuracy, latency metrics, and Raspberry Pi deployment steps.

smart_agriculture_concept.md

Part 2 (Task 2): Design document for the AI-IoT Agriculture system (Sensors, Model, DFD).

Part 1: Theoretical Analysis

File: theoretical_analysis.md

This document addresses the theoretical essay questions:

Edge AI vs. Cloud AI: Explains how processing data locally reduces latency (e.g., in autonomous drones) and enhances privacy by keeping raw data off the cloud.

Quantum AI vs. Classical AI: Compares binary bit processing with quantum superposition for optimization problems, highlighting benefits for industries like logistics and pharmaceuticals.

Part 2: Practical Implementation

Task 1: Edge AI Prototype

Files: edge_ai_prototype.py, edge_ai_report.md

A functional implementation of an Edge AI image classifier for waste sorting ("Recyclable" vs. "Organic").

How to Run the Code:

Ensure you have Python installed with the necessary libraries:

pip install tensorflow numpy matplotlib


Run the script:

python edge_ai_prototype.py


What happens:

The script downloads the CIFAR-10 dataset (used as a proxy for waste images).

It trains a lightweight Convolutional Neural Network (CNN).

It converts the model to a quantized TensorFlow Lite (.tflite) file.

It runs a simulated inference test to measure latency (speed) and accuracy.

Deployment:
Refer to edge_ai_report.md for specific instructions on how to load the generated .tflite model onto a Raspberry Pi using the tflite-runtime library.

Task 2: AI-Driven IoT Concept

File: smart_agriculture_concept.md

A system design for a Smart Agriculture environment.

Key Components:

Sensors: Soil Moisture, DHT22 (Temp/Humidity), NPK, Light (PAR), and pH sensors.

AI Model: A Random Forest Regressor designed to predict crop yields based on soil and weather data.

Data Flow: A Mermaid diagram visualizing the path from Sensor $\to$ Microcontroller $\to$ Cloud AI $\to$ Dashboard/Actuator.

Prerequisites for Deployment

If you intend to deploy the solution physically (Task 2) or run the inference on an actual Edge device (Task 1), you will need:

Hardware: Raspberry Pi 4 (or similar), ESP32 Microcontroller.

Sensors: Capacitive Soil Moisture Sensor, DHT22.

Software: Python 3.7+, TensorFlow Lite Runtime (tflite_runtime).
