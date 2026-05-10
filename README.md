# BrainBoard

Welcome to the **BrainBoard** project repository. This project is a comprehensive Brain-Computer Interface (BCI) system developed by **KN Neuron** (Neuroinformatics Student Research Group, Wrocław University of Technology).

BrainBoard leverages EEG signals—specifically motor imagery (MI)—to drive a variety of applications, from experimental setups to a functional BCI keyboard. 

It was developed by:
- [Grzegorz Szczepanek](https://github.com/GrzegorzSzczepanek)
- [Mikołaj Popik](https://github.com/M1KUS3Q)
- [Tomasz Stefaniak](https://github.com/tomekstefaniak)
- [Wiktor Dembny](https://github.com/dembol23)
- [JuLa Szymańska](https://github.com/jszymanska14)

## 🚀 Project Components

This repository serves as a central hub for the following components, included as submodules:

### 1. [Motor Imagery AI](./motor-imagery-AI)
A modular Python pipeline for classifying motor imagery (left-hand, right-hand, and rest).
- **Dataset:** [PhysioNet EEG Motor Movement/Imagery Dataset](https://physionet.org/content/eegmmidb/1.0.0/).
- **Pipeline:** Includes data downloading, preprocessing, training loops, and cross-validation.
- **Goal:** To provide robust models for MI classification.

### 2. [Motor Imagery Experiment](./motor-imagery-experiment)
A Pygame-based experimental environment that integrates GUI, EEG headset, and data management.
- **GUI:** Immersive interface for users during BCI experiments.
- **Integration:** Seamlessly connects with EEG headsets for real-time data acquisition.
- **Hex-O-Spell:** Includes components for the Hex-O-Spell speller paradigm.

### 3. [BrainBoard Keyboard](./BrainBoard-Keyboard)
A functional motor-imagery BCI keyboard.
- **Input Signals:** Left-hand MI, right-hand MI, and deliberate eye blinks.
- **Architecture:** Features a BCI pipeline (EEGNet for MI, blink detection, smoothing/debounce) driving a sector/letter speller state machine.
- **Hardware Support:** Compatible with BrainAccess, BioAmp EXG, and MIDI/Mock playback.

## 🛠 Getting Started

To clone this repository along with all its submodules, use:

```bash
git clone --recursive https://github.com/KN-Neuron/Brainboard.git
```

If you have already cloned the repository, you can initialize and update the submodules with:

```bash
git submodule update --init --recursive
```

## 🧠 About KN Neuron
**KN Neuron** is a student research group at Wrocław University of Technology focused on neuroinformatics, brain-computer interfaces, and signal processing.

## 📄 License
This project is licensed under the terms of the LICENSE file found in the root directory.
