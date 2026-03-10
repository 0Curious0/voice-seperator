# Voice Separation using Independent Component Analysis (ICA)
# Overview

This project implements voice/source separation using Independent Component Analysis (ICA).

The goal is to recover individual audio signals from a mixture of multiple sources — a classic signal processing problem often referred to as the “cocktail party problem.”

Given recordings that contain multiple overlapping voices, the algorithm separates them into their original independent signals by exploiting statistical independence between sources.

This project was completed as part of a Stanford machine learning coursework assignment focused on unsupervised learning and blind source separation.


# Problem Statement

When multiple audio sources are recorded simultaneously by microphones, each microphone captures a mixture of the speakers' sounds.

But we want to seperate out the audio of each speaker.

# Mathematical Model

Let:  s = original source signals
      x = observed mixed signals
      A = unknown mixing matrix

The mixing process can be represented as: x=As

ICA estimates an unmixing matrix W such that: s≈Wx

The algorithm works by maximizing statistical independence between recovered components.


# Important Note About the Assignment

This implementation is based on a Stanford coursework assignment that provided partial starter code.

My contribution involved:

1. Implementing the core ICA algorithm
2. Completing missing functions
3. Implementing the optimization logic
4. Debugging and validating the separated signals

The starter framework and assignment description were provided by the course.

# Future Improvements

Possible extensions include:

1. Implementing FastICA for faster convergence
2. Separating more than two audio sources
3. Using real-world microphone recordings
4. Interactive visualization of signals during separation
