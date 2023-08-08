# RDM dataset

This dataset contains images of the CNR-STIIMA ReDeManufacturing Lab:
* [real data](RealData/) as pictures of real assets (e.g. pallet, PCBs)
* [synthetic data](SyntheticData/) generated using the [VR digital twin](https://difactory.github.io/DF/scenes/VL/RdmPlant.html) of the lab


## Real Data
Real data are provided in terms of two different datasets, **[DR0](RealData/DR0/)** and **[DR1](RealData/DR1/)**.


## Synthetic Data
Synthetic data are provided in terms of six different datasets:
* **[DS2](SyntheticData/DS2)**: images with the tree classes of objects on a grey or light grey background.
* **[DS3](SyntheticData/DS3)**: images with the tree classes of objects on white background.
* **[DS4](SyntheticData/DS4)**: images with the tree classes of objects on a black background.
* **[DS5](SyntheticData/DS5)**: images with the tree classes of objects (PCB, pallet, conveyor) placed in the realistic context, i.e., the virtual representation of the plant. 
* **[DS6](SyntheticData/DS6)**: images replicating the real configuration of the plant by including multiple instances of conveyors, pallets and PCBs.
* **[DS7](SyntheticData/DS7)**: images with PCBs and pallets, together with other objects that do must not be detected

## Annotations
Annotations linked to the images in the datasets are provided as a single annotation file, one for the real data and one for the synthetic data, containing:

* the name of the image file;
* a set of one or more blocks separated by a space, each containing 5 elements:
    * the coordinates of the bounding box (xmin, ymin, xmax, ymax);
    * the id of the class of object (0, 1 or 2).

The following classes of objects are taken into consideration
| ID | Description |
| --- | ----------- |
| 0 | Conveyor |
| 1 | Pallet |
| 2 | PCB  |
