# Render Area

The render area is the main area of the user interface where you can interact with the room and its objects. The render area is also where you can place, move, resize, and delete objects. The visual representation (the texture) of the render area scales with the size of the window. However the underlying data (the simulation itself) is done in a 700x700 grid. Due to this, artifacts may appear at some resolutions.

## Gizmos

Gizmos appear for each object, when you hover over the area. To get a better view of the simulation, you can hide the gizmos simply by hovering over a different area of the screen.

## Gradients

Rendering happens each frame of the UI-Thread (VSynced to your monitor, usually 60Hz). The simulation is done at a variable rate, chosen by you (see [Quick Settings](./quick_settings.md)). During rendering all pressure values in each cell of the grid are used to lookup a color in a gradient. The gradient can be changed in the [Preferences](./preferences.md).

## Gamma Correction

The pixel buffer used ([bevy_pixel_buffer](https://github.com/Zheoni/bevy_pixel_buffer)) for rendering is stroring pixel values in linear color space. This means that the colors are not gamma corrected. To correct this, a gamma correction is applied to the gradient colors using the gamma value 2.2.
