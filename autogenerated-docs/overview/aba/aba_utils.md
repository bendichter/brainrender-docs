# aba\_utils

## Contents

* [line: 28 - `parse_neurons_colors`](aba_utils.md#line-28---parse_neurons_colors)
* [line: 147 - `parse_tractography_colors`](aba_utils.md#line-147---parse_tractography_colors)
* [line: 243 - `experiments_source_search`](aba_utils.md#line-243---experiments_source_search)
* [line: 301 - `parse_streamline`](aba_utils.md#line-301---parse_streamline)
* [line: 378 - `make_url_given_id`](aba_utils.md#line-378---make_url_given_id)
* [line: 390 - `download_streamlines`](aba_utils.md#line-390---download_streamlines)
* [line: 430 - `extract_ids_from_csv`](aba_utils.md#line-430---extract_ids_from_csv)

## line: 28 - `parse_neurons_colors`

```text
def parse_neurons_colors(neurons, color):
```

> Prepares the color info to render neurons  
> :param neurons: str, list, dict. File\(s\) with neurons data or list of rendered neurons.  
> :param color: default None. Can be: - None: each neuron is given a random color - color: rbg, hex etc. If a single color is passed all neurons will have that color - cmap: str with name of a colormap: neurons are colored based on their sequential order and cmap - dict: a dictionary specifying a color for soma, dendrites and axon actors, will be the same for all neurons - list: a list of length = number of neurons with either a single color for each neuron or a dictionary of colors for each neuron

## line: 147 - `parse_tractography_colors`

```text
def parse_tractography_colors(tractography, include_all_inj_regions, color=None, color_by='manual', VIP_regions=[], VIP_color=None, others_color='salmon'):
```

> parses color arguments to render tracrography data  
> :param tractography: list of dictionaries with tractography data  
> :param color: color of rendered tractography data  
> :param color\_by: str, specifies which criteria to use to color the tractography \(Default value = "manual"\) Options: - manual: the user needs to provide a color or list of colors - target\_region: tracts are colored according to the region where the injection was done. if VIP\_regions is passed, then only tracts for the VIP regions are colored  
> :param VIP\_regions: list of brain regions with VIP treatement \(Default value = \[\]\)  
> :param VIP\_color: str, color to use for VIP data \(Default value = None\)  
> :param include\_all\_inj\_regions: bool \(Default value = False\)  
> :param others\_color: str, color for not VIP data \(Default value = "white"\)

## line: 243 - `experiments_source_search`

```text
def experiments_source_search(mca, SOI, *args, source=True, **kwargs):
```

> Returns data about experiments whose injection was in the SOI, structure of interest  
> :param SOI: str, structure of interest. Acronym of structure to use as seed for teh search  
> :param _args:  
> :param source: \(Default value = True\)  
> :param \*_kwargs:

## line: 301 - `parse_streamline`

```text
def parse_streamline(*args, filepath=None, data=None, show_injection_site=True, color='ivory', alpha=0.8, radius=10, **kwargs):
```

> Given a path to a .json file with streamline data \(or the data themselves\), render the streamline as tubes actors.Either filepath or data should be passed  
> :param filepath: str, optional. Path to .json file with streamline data \(Default value = None\)  
> :param data: panadas.DataFrame, optional. DataFrame with streamline data. \(Default value = None\)  
> :param color: str color of the streamlines \(Default value = 'ivory'\)  
> :param alpha: float transparency of the streamlines \(Default value = .8\)  
> :param radius: int radius of the streamlines actor \(Default value = 10\)  
> :param show\_injection\_site: bool, if True spheres are used to render the injection volume \(Default value = True\)  
> :param _args:  
> :param \*_kwargs:

## line: 378 - `make_url_given_id`

```text
def make_url_given_id(expid):
```

> Get url of JSON file for an experiment, give it's ID number  
> :param expid: int with experiment ID number

## line: 390 - `download_streamlines`

```text
def download_streamlines(eids, streamlines_folder=None):
```

> Given a list of expeirmental IDs, it downloads the streamline data from the [https://neuroinformatics.nl](https://neuroinformatics.nl) cache and saves them asjson files.  
> :param eids: list of integers with experiments IDs  
> :param streamlines\_folder: str path to the folder where the JSON files should be saved, if None the default is used \(Default value = None\)

## line: 430 - `extract_ids_from_csv`

```text
def extract_ids_from_csv(csv_file, download=False, **kwargs):
```

> Parse CSV file to extract experiments IDs and link to downloadable streamline dataGiven a CSV file with info about experiments downloaded from: [http://connectivity.brain-map.orgextract](http://connectivity.brain-map.orgextract) experiments ID and get links to download \(compressed\) streamline data from [https://neuroinformatics.nl.Also](https://neuroinformatics.nl.Also) return the experiments IDs to download data from: [https://neuroinformatics.nl/HBP/allen-connectivity-viewer/streamline-downloader.html](https://neuroinformatics.nl/HBP/allen-connectivity-viewer/streamline-downloader.html)  
> :param csv\_file: str with path to csv file  
> :param download: if True the data are downloaded automatically \(Default value = False\)  
> :param \*\*kwargs:

