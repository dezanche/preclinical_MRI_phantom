# preclinical_MRI_phantom
This modular phantom is designed for system calibration and quality assurance of preclinical (animal) MRI scanners. Unlike clinical (human-sized) systems, for which the [American College of Radiology](https://www.acr.org/) has standardized the phantoms and measurements, for preclinical applications phantoms with these capabilities do not exist.
This repository contains detailed information in support of the scientific abstract submitted to the [2022 ISMRM conference](https://www.ismrm.org/22m/).

## Contents
[CAD](./tree/main/CAD) contains CAD files describing the phantom as built.\
[Images](./tree/main/Images) contains the renderings and photographs shown below.

## Construction
The phantom as built is made using an off-the-shelf 50mL centrifuge tube as the outer container (inner diameter approximately 26 mm tapering down to 25 mm at the base), in which several 25 mm diameter modules are stacked to provide the features described below. These dimensions mimic those of a mouse; to mimic other animals the dimensions of the [CAD](./tree/main/CAD) objects can be scaled accordingly to fit a container with appropriate dimensions.
The remaining volume of the container is filled with the standard 7.8 mM CuSO<sub>4</sub> and 61.6 mM NaCl aqueous solution used in the [ACR phantoms](https://www.acraccreditation.org/-/media/ACRAccreditation/Documents/MRI/ACR-Large--Med-Phantom-GuidanceFinal.pdf) or other liquids that give NMR signal.

### Modules
The modules in the [CAD](./tree/main/CAD) drawing provide the following features:
1. Slice location: two sets of intersecting ramps angled at 90° to each other (tilted 45° from the axis in opposite directions).
2. Slice thickness: two sets of parallel planes tilted 10° from the transverse plane to de ne a thin slab from which the slice pro le is measured.
3. Slice angle: crossed triangular prisms to detect slice tilt (in which case the arms of the resulting cross in the image are not parallel).
4. Radial resolution : 36 radially-oriented spokes (5° wedges) taper down to 50 μm.
5. Linear resolution: two sets of rectangular slots ranging from 0.5 mm to 50 μm in width.
6. Low-contrast resolution: holes of di erent sizes in disks thinner than the slices acquired.
7. Distortion grid: rectangular grid of holes in a material at least as thick as the slices acquired.
8. Spacer: annulus or ring of uniform thickness maintains adjacent modules parallel and provides a region of uniform signal for measurements such as
image uniformity and SNR.

## License
