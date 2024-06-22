# Setting-Up-Ollama-Locally
Steps to set up Ollama locally on my computer (llama3, llama2, Mistral, Phi, Gemma:2b)
# Local Model Setup with Ollama

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Model Setup](#model-setup)
   - [Llama 3](#llama-3)
   - [Llama 2](#llama-2)
   - [Mistral](#mistral)
   - [Phi](#phi)
   - [Gemma](#gemma)
5. [Running Models](#running-models)
6. [Usage Examples](#usage-examples)
7. [Troubleshooting](#troubleshooting)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction
This repository provides instructions and scripts to set up various language models locally using Ollama. The models covered include Llama 3, Llama 2, Mistral, Phi, and Gemma (gemma:2b). 

## Prerequisites
Before you begin, ensure you have the following:
- A computer with macOS, Windows, or Linux.
- Python 3.8 or higher installed.
- Docker installed (optional but recommended for containerized environments).

## Installation
Follow these steps to install Ollama and necessary dependencies:

1. **Clone the Repository**
    ```sh
    git clone https://github.com/ollama/ollama.git
    cd ollama
    ```

2. **Install Ollama**
    ```sh
    pip install ollama
    ```

## Model Setup

### Llama 3
1. **Download Llama 3**
    ```sh
    ollama pull llama3
    ```

2. **Configuration**
    Create a configuration file named `llama3_config.json`:
    ```json
    {
        "model": "llama3",
        "version": "latest"
    }
    ```

### Llama 2
1. **Download Llama 2**
    ```sh
    ollama pull llama2
    ```

2. **Configuration**
    Create a configuration file named `llama2_config.json`:
    ```json
    {
        "model": "llama2",
        "version": "latest"
    }
    ```

### Mistral
1. **Download Mistral**
    ```sh
    ollama pull mistral
    ```

2. **Configuration**
    Create a configuration file named `mistral_config.json`:
    ```json
    {
        "model": "mistral",
        "version": "latest"
    }
    ```

### Phi
1. **Download Phi**
    ```sh
    ollama pull phi
    ```

2. **Configuration**
    Create a configuration file named `phi_config.json`:
    ```json
    {
        "model": "phi",
        "version": "latest"
    }
    ```

### Gemma
1. **Download Gemma**
    ```sh
    ollama pull gemma:2b
    ```

2. **Configuration**
    Create a configuration file named `gemma_config.json`:
    ```json
    {
        "model": "gemma",
        "version": "2b"
    }
    ```

## Running Models
To run any of the models, use the following command structure:
```sh
ollama run -c <config_file>






##### Running simple commands using curl

curl -X POST http://localhost:11434/api/generate -d '{
  "model": "llama3",
  "prompt": "Why is the sky blue?"
}'




####Troubleshooting
If you face problems, consider the following:

Ensure that all dependencies are installed.
Check that the configuration files are correctly set up.
Check for error messages in the terminal.


