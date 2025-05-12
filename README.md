# How to Print Your Marker: an Open-Source, Easy-to-Make, Compact Active Wireless Marker for Motion Tracking


Released CAD for the wireless marker design presented at ISMRM 2025 (Abstract #4589):

A. De Goyeneche, J. Maravilla, K. Gopalan, A. Falk, S. Yu, C. Liu, M. Lustig. “How to Print Your Marker: an Open-Source, Easy-to-Make, Compact Active Wireless Marker for Motion Tracking”. *Proceedings of the 34th Annual Meeting of ISMRM, Honolulu, Hawaii, USA, 2025.* 

This repository provides an easy-to-assemble, compact, open-source 3D-printed marker housing for use in MRI applications.  
It is designed to support existing wireless RF marker circuits based on inductive coupling, and simplifies construction for broader use and reproducibility.


## Overview

![Markers Overview](figures/marker_cad.png)


- Compact design (<11 × 7 × 6 mm).
- Two-part SLA-printed shell.
- Cavity for Gd-doped water signal source.
- Passive detuning using crossed diodes.
- Rapid localization using projection acquisitions.



### Bill of materials

- Enamel-insulated copper wire.
- SMD 1111 form factor capacitor (we used 39 pF to tune to ~127.7MHz).
- 2x MA4P7446F for crossed diodes.
- SLA 3D printer (we used clear resin).
- Gd-doped water solution (e.g. 10nM for ~5ms T1 and T2).
- UV glue or sealant.


### Assembly instructions 

![Assembly Steps](figures/steps.png)


1. **3D Print** the two-piece shell. 
1. **Coil the wire**: Loop the wire three times along the groove around the spherical cavity on the base piece. Expose the wire sections by the components compartment. Trim the wire ends to align with the end of the component-holding structure on each side.
1. **Assemble**: Place the capacitor on the base piece and the crossed diodes on the cap piece. 
1. **Close & Solder**: Fit the cap onto the base and obtain a tight fit with a vise or similar tool. Apply flux to the exposed wire and components and solder each side. Clear print resin is useful for observing the solder flow and ensuring a complete connection.
1. **Tune**: Using a Vector Network Analyzer (VNA), slightly adjust the spacing between coil turns to tune the marker to the desired frequency (e.g., looking for a dip in S11 at ~127.7 MHz).
1. **Fill & Seal**: Fill the cavity with Gd-doped water solution through the top hole and seal it (e.g., using UV-curable glue). Re-tune if necessary.


### Citation

If you use or adapt this design, please cite:

A. De Goyeneche et al., “How to Print Your Marker: an Open-Source, Easy-to-Make, Compact Active Wireless Marker for Motion Tracking.” ISMRM 2025, Abstract #4589.


### License

Licensed under CC BY-NC 4.0 — for non-commercial research use only.

[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc/4.0/)
