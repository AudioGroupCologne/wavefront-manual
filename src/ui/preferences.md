# Preferences

The preferences window provides more customization options compared to the [quick settings](../ui/quick_settings.md) panel.

## General Settings

The general settings allow modification of simulation as well as rendering behavior.

### Simulation

The `Delta L (m)` slider sets the distance between pixels in real world scale. Smaller distances correspond to a smaller area. 

The `Show absorbing boundary` toggle displays the absorbing boundary around the simulation area. The absorbing boundary is used for more accurate free field simulations. The absorbing boundary width is modified with the `Boundary width (px)` slider. Greater values correspond to better free field simulations (the free field works best for wavelengths shorter than the boundary width).

### Rendering

The `Colormap` drop-down list allows the selection of multiple different gradients for rendering. The most common scientific gradients are represented.

The `Min Gradient` and `Max Gradient` values set the minimum and maximum pressure values. Greater and smaller values are clipped at the gradients edges.

## Experimental Settings

Experimental settings offer toggles for experimental features which are disabled / hidden by default. These features might be incomplete, broken or subject to change in the future.

The `Frequency analyzer` toggle enables the use of the [frequency plot](./plots/frequency.md). There is a known bug in the analysis of white noise or Gaussian sources post-diffraction, characterized by the emergence of unexplainable high-frequency components.

The `Export CSV` toggle enables the export of the simulation data to a CSV file. The CSV file contains the pressure field measured by one microphone at each time step. The export is done in the background and the file is saved in the current working directory.
