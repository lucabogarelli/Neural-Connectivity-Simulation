# Inhibitory Synapses and Postsynaptic Neuron Dynamics

## Overview
This project investigates the effect that the total number of inhibitory synaptic connections has on postsynaptic cell activity within a neuronal network. The **Brain Scaffold Builder (BSB)** framework is utilized to generate and simulate the activity of simplified bilayer networks composed of **Stellate** and **Purkinje** cell layers.

## Methodology & Network Variations
To experimentally evaluate the importance of connectivity magnitude on synaptic interactions, the project examines the spatio-temporal complexity of the networks' responses to a constant stimulus. The simulation compares three distinct connectivity strategies:
* **Low connectivity network:** Exhibits a lack of integration, implemented through a very low number of synapses.
* **Medium connectivity network:** Connections are both integrated and specialized, linked with synapses that are realistic in both number and placement.
* **High connectivity network:** Exhibits a lack of specialization, implemented through an excessive number of synapses.

## Structure & Placement
* **Dimensions:** The network features a bilayer structure with overall dimensions of $200 \times 200 \times 200\ \mu m$, where each layer has a thickness of $100\ \mu m$.
* **Cell Populations:** The network contains **160 Stellate cells** in the first layer and **40 Purkinje cells** in the second layer.
* **Placement & Connectivity:** Cells are placed using BSB's `RandomPlacement` tool. Anatomically realistic synaptic connections are generated using the `VoxelIntersection` connectivity strategy, which leverages cell morphology and spatial placement.

## Requirements & Data Sources
* **Framework:** Brain Scaffold Builder (BSB).
* **Morphologies and Models:** Stellate and Purkinje cell morphologies (`.swc` files) and voltage models are downloaded directly from the `dbbs-lab/cerebellar-models` GitHub repository during the initial setup.

