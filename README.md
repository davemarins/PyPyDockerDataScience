# PyPy 3 Flask applications for data science

This folder is a project template for Python web applications powered by Flask web framework and PyPy 3.
The goal is to run a distributed application with REST paradigm in order to deploy
stable and fast code for data science purposes.

# Approach

PyPy is a JIT compiler for the Python language, but not all .whl are supported. When
it's not possible, a C++ daemon waits for events to occur; this project will have 2 engines
which communicates through Google protobuf (https://github.com/protocolbuffers/protobuf) in
order to transmit entire object or some complex data structure within this service.

# Data science approach

TODO: choose which operations will be done, partly in Python and C++
Pytorch model for OpenCV? spaCy? DeepSpeech?
