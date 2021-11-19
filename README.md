# preclinical_MRI_phantom
This modular phantom is designed for system calibration and quality assurance of preclinical (animal) MRI scanners. Unlike clinical (human-sized) systems, for which the [American College of Radiology](https://www.acr.org/) has standardized the phantoms and measurements, for preclinical applications phantoms with these capabilities do not exist.
This repository contains detailed information in support of the scientific abstract submitted to the [2022 ISMRM conference](https://www.ismrm.org/22m/).
![assembled phantom](https://github.com/dezanche/preclinical_MRI_phantom/blob/main/Images/Photos/phantom_cropped.jpg)

## Contents
[CAD](https://github.com/dezanche/preclinical_MRI_phantom/tree/main/CAD) contains mechanical design (CAD) files describing the phantom as built.\
[Images](https://github.com/dezanche/preclinical_MRI_phantom/tree/main/Images) contains the renderings and photographs shown above and below.

## Construction
The phantom as built is made using an off-the-shelf 50mL centrifuge tube as the outer container (inner diameter approximately 26 mm tapering down to 25 mm at the base), in which several 25 mm diameter modules are stacked to provide the features described below. These dimensions mimic those of a mouse; to mimic other animals the dimensions of the [CAD](./tree/main/CAD) objects can be scaled accordingly to fit a container with appropriate dimensions.
The remaining volume of the container is filled with the standard 7.8 mM CuSO<sub>4</sub> and 61.6 mM NaCl aqueous solution used in the [AAPM phantoms](https://www.aapm.org/pubs/reports/rpt_100.pdf), 10 mM NiCl<sub>2</sub> and 75 mM NaCl of the [ACR phantoms](https://www.acraccreditation.org/-/media/ACRAccreditation/Documents/MRI/ACR-Large--Med-Phantom-GuidanceFinal.pdf), or other liquids that provide NMR signal.

### Modules
The modules in the [CAD](https://github.com/dezanche/preclinical_MRI_phantom/tree/main/CAD) drawing provide the following features:
1. Slice location: two sets of intersecting ramps angled at 90° to each other (tilted 45° from the axis in opposite directions).
2. Slice thickness: two sets of parallel planes tilted 10° from the transverse plane to de ne a thin slab from which the slice pro le is measured.
3. Slice angle: crossed triangular prisms to detect slice tilt (in which case the arms of the resulting cross in the image are not parallel).
4. Radial resolution: 36 radially-oriented spokes (5° wedges) taper down to 50 μm.
5. Linear resolution: two sets of rectangular slots ranging from 0.5 mm to 50 μm in width.
6. Low-contrast resolution: holes of different sizes in disks thinner than the slices acquired.
7. Distortion grid: rectangular grid of holes in a material at least as thick as the slices acquired.
8. Spacer: annulus or ring of uniform thickness maintains adjacent modules parallel and provides a region of uniform signal for measurements such as
image uniformity and SNR.

<!-- end of the list -->

![modules](https://github.com/dezanche/preclinical_MRI_phantom/blob/main/Images/Renderings/Modules.png)

All modules are designed with multiple points of contact to the adjacent modules to maintain parallel alignment. To facilitate filling, modules 4 and 5
include four semicircular passages at the periphery. Care must be taken to ensure that air bubbles are not trapped in the fine features of the modules or
between modules.

![modules](https://github.com/dezanche/preclinical_MRI_phantom/blob/main/Images/Renderings/mouse_phantom_exploded_view.png)

### Fabrication
Modules 1-5 were 3D printed using stereolithography because its resolution and fidelity (nominally 50 μm for our supplier) are superior to those of the
more common fused deposition modelling process. Modules 6 and 7 were milled using an LPKF ProtoMat S62 out of 0.8 mm FR4 (0.5 mm ⌀ holes, 1 mm
pitch) and thin (0.1 and 0.35 mm) plastic sheets, respectively. Module 7 was also made from a standard perforated prototyping printed circuit
board (FR4 without copper pads or traces) resulting in a coarser (2.54 mm pitch) grid.\
The spacer (8) is used to separate modules and to provide regions of uniform signal. In this implementation the spacers were standard R17 rubber o-
rings, but they can also be off-the-shelf nonmetallic washers, 3D printed or machined using standard techniques.
![modules](https://github.com/dezanche/preclinical_MRI_phantom/blob/main/Images/Photos/various_inserts.jpg)
![modules](https://github.com/dezanche/preclinical_MRI_phantom/blob/main/Images/Photos/resolution_inserts.jpg)

## Licenses
[CAD](https://github.com/dezanche/preclinical_MRI_phantom/tree/main/CAD) files are licensed under ... Additional license information is provided in that folder.\
All other original content in this repository (including this README file) is licensed under the CC...
