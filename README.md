# Online Event-Triggered Switching for Frequency Control in Power Grids with Variable Inertia

This repository contains the code for the paper **"Online Event-Triggered Switching for Frequency Control in Power Grids with Variable Inertia"**, submitted to *Transactions on Power Systems*.

## Project Overview

This project implements a Neural-PI controller framework for frequency control in power grids with variable inertia. The framework uses reinforcement learning to train controllers that adaptively switch based on system events, ensuring stability and performance under varying conditions.

## Repository Structure

- **`online-event-triggered-switching-neural-pi.ipynb`**: Jupyter notebook containing the main code for training and evaluating the Neural-PI controllers.
- **`data/`**: Directory containing the simulation data, such as the IEEE 39-bus system data.
- **`checkpoints/`**: Directory containing trained model checkpoints.

## Prerequisites

To run the code in this repository, you will need the following libraries:

- `matplotlib`
- `numpy`
- `tensorflow`
- `networkx`
- `scipy`
- `mat4py`
- `pickle`
- `time`

You can install the required libraries using pip:
```bash
pip install matplotlib numpy tensorflow networkx scipy mat4py
```

## Usage

1. **Set Up the Environment**: Ensure you have a suitable Python environment with the required libraries installed.

2. **Load the Notebook**: Open the `online-event-triggered-switching-neural-pi.ipynb` notebook in Jupyter.

3. **Run the Cells**: Execute the cells in the notebook to train the Neural-PI controllers and evaluate their performance on the provided simulation data.

## Key Components

### Frequency Control Environment

The `Frequency` class in the notebook defines the environment for the frequency control problem. It initializes system parameters and defines the state transition dynamics.

### Simulation Data

Simulation data is loaded from the IEEE 39-bus system using the `mat4py` library. Key parameters include system inertia, damping, and network topology.

### Training and Evaluation

The notebook provides a detailed implementation of the training procedure for the Neural-PI controllers, including the reinforcement learning setup and evaluation metrics.

## Results

The notebook includes plots and metrics to demonstrate the performance of the trained controllers under different inertia modes. The best performance for each mode is highlighted in bold in the results section.

## Citation

If you use this code in your research, please cite our paper once it is published.

<!-- ```bibtex
@article{author2024online,
  title={Online Event-Triggered Switching for Frequency Control in Power Grids with Variable Inertia},
  author={Your Name and Co-authors},
  journal={Transactions on Power Systems},
  year={2024}
}
``` -->

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

