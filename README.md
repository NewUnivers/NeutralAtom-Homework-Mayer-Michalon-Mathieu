# Neutral Atom Simulation Notebook

## Overview
This Jupyter Notebook, **Neutral Atom Simulation**, demonstrates the use of Pulser for simulating quantum systems using neutral atom registers. The notebook integrates tools from the Pulser framework to:

- Define and manipulate atomic registers.
- Simulate quantum sequences and dynamics.
- Solve graph problems (e.g., Maximum Independent Set, graph coloring).
- Visualize and analyze quantum results.

## Features
- physical_coords_to_atom_dict: Converts physical coordinates into scaled atomic positions for simulation.
- dict_to_graph: Constructs a graph where nodes are qubits and edges represent interference based on a given radius.
- define_sequence: Creates a quantum sequence with configurable pulses for simulation.
- MIS_adiabatic_solving: Implements an adiabatic quantum algorithm to solve the Maximum Independent Set problem.
- solve_graph_colouring: Solves the graph coloring problem using the MIS approach and assigns colors to nodes.

## Prerequisites

### Required Libraries
The following Python libraries are required:

```python
from pulser import Pulse, Sequence, Register, waveforms
from pulser.devices import MockDevice
from pulser_simulation import QutipEmulator, SimConfig
import numpy as np
import networkx as nx

