# llama-cpp-python CUDA Build for RTX 5070 Ti

This repository contains a GitHub Actions workflow to build `llama-cpp-python` wheels with CUDA support for the **NVIDIA GeForce RTX 5070 Ti (Blackwell)**.

## Prerequisites

- A GitHub repository where you can run GitHub Actions.
- A Blackwell GPU (RTX 50-series) to use the resulting wheels.

## How to Build

1. Push this repository to GitHub.
2. Go to the **Actions** tab in your GitHub repository.
3. Select the **Build llama-cpp-python for RTX 5070 Ti (Blackwell)** workflow.
4. Click **Run workflow**.
5. (Optional) Specify a specific `llama-cpp-python` version and `CUDA` version (default is CUDA 12.8.0).
6. Once the workflow finishes, download the `.whl` files from the **Artifacts** section.

## How to Install

Download the appropriate wheel for your Python version and operating system, then install it using pip:

```bash
# Example for Windows, Python 3.12
pip install llama_cpp_python-0.3.7-cp312-cp312-win_amd64.whl
```

## Configuration Details

- **Compute Capability:** 12.0 (Blackwell)
- **CUDA Architecture:** `120`
- **Minimum CUDA Toolkit:** 12.8.0
