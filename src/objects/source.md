# Source

Sources are the only sound emitters available in wavefront. They emit sound in all 4 directions (top, left, right, bottom) and can be placed anywhere in the [render area](../ui/render_area.md). Each source is can be assigned a number of properties such as frequency, amplitude and phase depending on the waveforms used.

The following waveforms are available for sources:

- [Sine](#sine)
- [Gaussian](#gaussian)
- [White Noise](#white-noise)

## Sine

The sine waveform is a simple waveform that oscillates in the range of \\([-a, a]\\) (where \\(a\\) is the amplitude). It is the most basic waveform and is used to represent a pure tone. The following parameters can be set for the sine waveform:

- Frequency: The frequency of the sine wave in Hz.
- Amplitude: The amplitude of the sine wave (unitless).
- Phase: The phase of the sine wave in degrees.

## Gaussian

The Gaussian waveform is a periodic bell-curve that is used to represent a short impulse. The following parameters can be set for the Gaussian waveform:

- Frequency: The frequency of the curve in Hz.
- Amplitude: The amplitude of the curve (unitless).
- Phase: The phase of the curve in degrees.
- Standard Deviation: The standard deviation (_width_) of the Gaussian curve.

## White Noise

The white noise outputs random noise at all frequencies. The following parameters can be set for the white noise waveform:

- Amplitude: The amplitude of the noise (unitless).
