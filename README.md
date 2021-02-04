# Video Analytics : Vehicle-Detection-Counting

Welcome to the Video Analytic repository for the vehicle-Detection-Counting challenges . This repo contains the definition of the environment where your code submissions will run. 

 ----

### [Getting started](#0-getting-started)
 - [Prerequisites](#prerequisites)
 - [Quickstart](#quickstart)
### [Testing your submission.zip](#1-testing-your-submissionzip)
 - [Implement your solution](#implement-your-solution)
 - [How your submission will run](#how-your-submission-will-run)
 - [Test running your submission locally](#test-running-your-submission-locally)
   - [Making a submission](#making-a-submission)
   - [Reviewing the logs](#reviewing-the-logs)
### [Updating the runtime packages](#2-updating-the-runtime-packages)
 - [Adding new Python packages](#adding-dependencies-to-the-runtime)
 - [Testing new dependencies](#testing-new-dependencies)
 - [Submitting a PR](#opening-a-pull-request)



----

## (0) Getting started

### Prerequisites

Make sure you have the prerequisites installed.

 - A clone or fork of this repository
 - [Docker](https://docs.docker.com/get-docker/)
 - At least ~10GB of free space for both the training images and the Docker container images
 - GNU make (optional, but useful for using the commands in the Makefile)
 - [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html) (Optional, but useful for the `make sample-images` command which downloads images from S3)

Additional requirements to run with GPU:
 - [NVIDIA drivers](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#package-manager-installation) (we check whether you have `nvidia-smi` installed and enabled to automatically determine whether to build the cpu or gpu image)
 - [NVIDIA Docker container runtime](https://nvidia.github.io/nvidia-container-runtime/)
