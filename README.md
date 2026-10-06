# DIY Oscilloscope
 
An ESP32-based DIY oscilloscope.

## Analogue front end
An ESP32's ADC only accepts 0-3.3 V, so to probe ±30 V, two inverting op-amps scale the signal down and lift it by ~1.65 V. A TVS diode, series resistor and Schottky clamps protect the ADC.

### LTspice
 
![LTspice circuit](docs/images/ltspicecircuit.png)
![LTspice simulation](docs/images/ltspicesim.png)

±30 V in (green), 0-3.3 V out (blue).
 
### KiCad
 
![Schematic](docs/images/kicadscheme.png)
![PCB layout](docs/images/kicadpcb.png)
![3D view](docs/images/kicadpcb3d.png)
 
## References
- [Qasim Asghar](https://www.youtube.com/watch?v=ud-KkpsHcRo)
