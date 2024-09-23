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

The `Mic values export` toggle adds an `Export CSV` button to each microphone entry in the [outline](./outline.md) panel. This button exports all recorded pressure values into a `.csv` file.

The `Wave files` toggle loads a `.wav` file and sets the `delta l` value to the corresponding sample rate. Each source now supports the `Wave file` waveform. Selecting this waveform type makes the source use the loaded wave file as an input. The simulation time controls the playback time of the audio file. A new `Export wav` button is also added to each microphone entry in the [outline](./outline.md) panel. This button export all recorded pressure values into a wave file.