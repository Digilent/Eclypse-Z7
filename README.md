# Eclypse Z7 Unifying Repository

## Description

This repository is designed to offer a unifying and comprehensive aproch to all the aspects that we provide, across multiple tools, for the Eclypse Z7. By cloning this repo recursively you will receive the repositories for the Viavdo project (HW), SDK workspace (SW) and Petalinux project (OS). Each submodule has it's own submodule dependencies which will be also pulled at cloning. An important aspect of this structure is the fact that both the SW and the OS are heavily depended on the hardware hand-off from the HW repository.

Each branch of this repository represents a different project with preset functionality. When checking out a branch all the submodules will be automatically configured to the same branch, thus providing a unified flow between all the submodules. For details about the individual functionality of the submodules please refer to the README.md files within the submodules.

For a detailed structural description of this repository and it's submodules, along with the branching system, please visit [Eclypse Z7 Git Repositoies](https://reference.digilentinc.com/reference/programmable-logic/eclypse-z7/git).

## First and Foremost

* The Vivado and Petalinux projects are version-specific. Source files are not backward compatible and not automatically forward compatible. Release tags specify the targetted Vivado version. There is only one version targetted per year, as chosen by Digilent. Non-tagged commits on the master branch are either at the last tagged version or the next targeted version. This is not ideal and might be changed in the future adopting a better flow.

* Our projects use submodules to bring in libraries. Use --recursive when cloning or `git submodule init` and `git submodule update`, if cloned already non-recursively.

## Requirements

Depending on which parts and branches of the this repository will be used the following will be needed to get it working:

* **Eclypse Z7**
* **Zmod ADC 1410**
* **Zmod DAC 1411**

HW/SW:

* **Vivado 2019.1 Installation with Xilinx SDK**: To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).

OS:

* **Petalinux 2019.1**: For installation, please follow the user guide provided by Xilinx [Petalinux Reference Guide (UG1144)](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2019_1/ug1144-petalinux-tools-reference-guide.pdf).


## Setup

No setup is needed at this stage, please refer to the individual README.md of each submodule on each branch for a more details.

We provide a ready to use [SD card image](https://github.com/Digilent/Eclypse-Z7/releases) with a Debian 10 Linux distribution, based on the OS repository, custom tailored for the Eclypse Z7 with Zmods in the release section of this repository.

## Additional Notes

For more information on the Eclypse Z7, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/eclypse-z7/start) on the Digilent Wiki.

For more information on the Zmod ADC 1410, please visit its [Resource Center](https://reference.digilentinc.com/reference/zmod/zmodadc/start) on the Digilent Wiki.

For more information on the Zmod DAC 1411, please visit its [Resource Center](https://reference.digilentinc.com/reference/zmod/zmoddac/start) on the Digilent Wiki.

For more information on how our git and project flow is set up, please refer to the [Eclypse Z7 Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/eclypse-z7/git) documentation.

For more information on how Vivado project is version controlled, refer to the [digilent-vivado-scripts repo](https://github.com/digilent/digilent-vivado-scripts).

For more details on how to use the [zmodlib](https://github.com/Digilent/zmodlib) and for instructions on how to set up your environment please visit the [Zmod Base Library User Guide](https://reference.digilentinc.com/reference/zmod/zmodbaselibraryuserguide)

For information related to Petalinux, please visit [Petalinux Reference Guide (UG1144)](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2019_1/ug1144-petalinux-tools-reference-guide.pdf)


For technical support or questions, please post on the [Digilent Forum](forum.digilentinc.com).
