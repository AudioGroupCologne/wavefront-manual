# Walls

Walls can be placed in the simulation area. In this version of wavefront there are two primitive types of walls: rectangles and circles. Walls can be placed using the [place](../tools/place.md) tool.

All wall types have the following properties:
- Reflection factor (0-1): The reflection factor determines how much of the wave is reflected when it hits the wall. A reflection factor of 0 means that the wave is absorbed completely, while a reflection factor of 1 means that the wave is reflected completely.
- Hollow (true/false): If a wall is hollow, wave propagation is allowed inside of the wall. This can be useful for creating complex waveguides or rooms.

## Rectangle Walls

Rectangular walls are defined by two points: the top-left and bottom-right corners of the rectangle. The reflection factor and hollow properties are applied to the entire rectangle.

## Circle Walls

Circular walls are defined by a center point and a radius. The reflection factor and hollow properties are applied to the entire circle.
