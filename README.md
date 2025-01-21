[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14709022.svg)](https://doi.org/10.5281/zenodo.14709022)

[contributors-shield]: https://img.shields.io/github/contributors/bvhpatel/TD-pressure-flow-paper-code.svg?style=flat-square
[contributors-url]: https://github.com/bvhpatel/TD-pressure-flow-paper-code/graphs/contributors
[stars-shield]: https://img.shields.io/github/stars/bvhpatel/TD-pressure-flow-paper-code.svg?style=flat-square
[stars-url]: https://github.com/bvhpatel/TD-pressure-flow-paper-code/stargazers
[issues-shield]: https://img.shields.io/github/issues/bvhpatel/TD-pressure-flow-paper-code.svg?style=flat-square
[issues-url]: https://github.com/bvhpatel/TD-pressure-flow-paper-code/issues
[license-shield]: https://img.shields.io/github/license/bvhpatel/TD-pressure-flow-paper-code.svg?style=flat-square
[license-url]: https://github.com/bvhpatel/TD-pressure-flow-paper-code/blob/master/LICENSE

# Code: Thoracic duct pressure flow relation paper

## About
This is the code associated with our paper where we derived a mathematical model for the pressure-flow relationship for a thoracic duct segment with one valve. See this [inventory](https://github.com/bvhpatel/TD-pressure-flow-paper-inventory) for all related resources, including the paper.


## Standards followed
The overall code is structured according to the [FAIR-BioRS guidelines](https://doi.org/10.1038/s41597-023-02463-x). The Python code in the Jupyter notebook follows the [PEP8 guidelines](https://peps.python.org/pep-0008). All the dependencies are documented in the [environment.yml](environment.yml) file.

## Using the Jupyter notebooks

### Prerequisites 
We recommend using Anaconda to create and manage your development environment and using JupyterLab to run the notebook. All the subsequent instructions are provided assuming you are using [Anaconda (Python 3 version)](https://www.anaconda.com/products/individual) and JupyterLab.

### Clone repo
Clone the repo or download as a zip and extract.

### cd into the code folder

Open Anaconda prompt (Windows) or the system Command line interface then naviguate to the code
```sh
cd .TD-pressure-flow-paper-code

```

### Setup conda env
```sh
$ conda env create -f environment.yml
```

### Setup kernell for Jupyter lab
```sh
$ conda activate TD-paper-env
$ conda install ipykernel
$ ipython kernel install --user --name=TD-paper
$ conda deactivate
```

### Launch Jupyter lab
Launch Jupyter lab and naviguate to open the Jupyter notebook. Make sure to change the kernel to the one created above called "TD-paper" (e.g., see [here](https://doc.cocalc.com/howto/jupyter-kernel-selection.html#cocalc-s-jupyter-notebook)). We recommend to use the [JupyterLab code formatter](https://github.com/ryantam626/jupyterlab_code_formatter) along with the [Black](https://github.com/psf/black) and [isort](https://github.com/PyCQA/isort) formatters to facilitate compliance with PEP8 if you are editing the notebook.

## Inputs/outputs
The Jupyter notebook makes use of the dataset in the dataset associated with the paper [(see here)](https://github.com/bvhpatel/TD-pressure-flow-paper-inventory). You will need to download the dataset spreadsheet at add it in the [inputs](inputs) folder.

Outputs of the code include plots and tables displayed in the notebook but also saved as files. These saved plot files are included in the [outputs](outputs) folder. 

## License
This work is licensed under
[MIT](https://opensource.org/licenses/mit). See [LICENSE](LICENSE) for more information.

## Feedback and contribution
Use the [GitHub issues](https://github.com/bvhpatel/TD-pressure-flow-paper-code/issues) for submitting feedback or making suggestions. You can also work the repository and submit a pull request with suggestions.

## How to cite
If you use this code, please cite the related paper (it will be listed [here](https://github.com/bvhpatel/TD-pressure-flow-paper-inventory) when available) and also cite this repository as:

```bash
Patel, Bhavesh, Aashish Ahuja, Ghassan Kassab. Code: Thoracic duct pressure flow relation paper [Software]. Zenodo. https://doi.org/10.5281/zenodo.14709022
