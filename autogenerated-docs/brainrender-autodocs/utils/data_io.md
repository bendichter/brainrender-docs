# data\_io

## Contents

* [**`listdir`** \[\#15\]](data_io.md#listdir-15)
* [**`get_subdirs`** \[\#28\]](data_io.md#get_subdirs-28)
* [**`check_file_exists`** \[\#35\]](data_io.md#check_file_exists-35)
* [**`get_file_name`** \[\#45\]](data_io.md#get_file_name-45)
* [**`load_npy_from_gz`** \[\#51\]](data_io.md#load_npy_from_gz-51)
* [**`save_npy_to_gz`** \[\#56\]](data_io.md#save_npy_to_gz-56)
* [**`save_json`** \[\#62\]](data_io.md#save_json-62)
* [**`save_yaml`** \[\#81\]](data_io.md#save_yaml-81)
* [**`load_json`** \[\#103\]](data_io.md#load_json-103)
* [**`load_yaml`** \[\#117\]](data_io.md#load_yaml-117)
* [**`load_volume_file`** \[\#131\]](data_io.md#load_volume_file-131)
* [**`load_mesh_from_file`** \[\#149\]](data_io.md#load_mesh_from_file-149)
* [**`connected_to_internet`** \[\#180\]](data_io.md#connected_to_internet-180)
* [**`send_query`** \[\#196\]](data_io.md#send_query-196)
* [**`get_probe_points_from_sharptrack`** \[\#215\]](data_io.md#get_probe_points_from_sharptrack-215)

## **`listdir`** \[\#15\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L15) online

```python
def listdir(fld):
```

   
docstring:

```text
List the files into a folder with the coplete file path instead of the
    relative file path like os.listdir.

:param fld: string, folder path
```

## **`get_subdirs`** \[\#28\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L28) online

```python
def get_subdirs(folderpath):
```

   
docstring:

```text
Returns the subfolders in a given folder
```

## **`check_file_exists`** \[\#35\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L35) online

```python
def check_file_exists(filepath, raise_error=False):
```

   
docstring:

no docstring

## **`get_file_name`** \[\#45\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L45) online

```python
def get_file_name(filepath):
```

   
docstring:

no docstring

## **`load_npy_from_gz`** \[\#51\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L51) online

```python
def load_npy_from_gz(filepath):
```

   
docstring:

no docstring

## **`save_npy_to_gz`** \[\#56\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L56) online

```python
def save_npy_to_gz(filepath, data):
```

   
docstring:

no docstring

## **`save_json`** \[\#62\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L62) online

```python
def save_json(filepath, content, append=False):
```

   
docstring:

```text
Saves content to a JSON file

:param filepath: path to a file (must include .json)

:param content: dictionary of stuff to save
```

## **`save_yaml`** \[\#81\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L81) online

```python
def save_yaml(filepath, content, append=False, topcomment=None):
```

   
docstring:

```text
Saves content to a yaml file

:param filepath: path to a file (must include .yaml)

:param content: dictionary of stuff to save
```

## **`load_json`** \[\#103\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L103) online

```python
def load_json(filepath):
```

   
docstring:

```text
Load a JSON file

:param filepath: path to a file
```

## **`load_yaml`** \[\#117\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L117) online

```python
def load_yaml(filepath):
```

   
docstring:

```text
Load a YAML file

:param filepath: path to yaml file
```

## **`load_volume_file`** \[\#131\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L131) online

```python
def load_volume_file(filepath):
```

   
docstring:

```text
Load a volume file (e.g., .nii) and returns the data

:param filepath: path to file

:param **kwargs:
```

## **`load_mesh_from_file`** \[\#149\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L149) online

```python
def load_mesh_from_file(filepath, *args, **kwargs):
```

   
docstring:

```text
Load a a mesh or volume from files like .obj, .stl, ...

:param filepath: path to file

:param **kwargs:
```

## **`connected_to_internet`** \[\#180\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L180) online

```python
def connected_to_internet(url='http://www.google.com/', timeout=5):
```

   
docstring:

```text
Check that there is an internet connection

:param url: url to use for testing (Default value =
    'http://www.google.com/')

:param timeout:  timeout to wait for [in seconds] (Default value = 5)
```

## **`send_query`** \[\#196\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L196) online

```python
def send_query(query_string, clean=False):
```

   
docstring:

```text
Send a query/request to a website

:param query_string: string with query content

:param clean:  (Default value = False)
```

## **`get_probe_points_from_sharptrack`** \[\#215\]

Check the [_**`source code`**_](https://github.com/BrancoLab/BrainRender/tree/brainglobeintegration/blob/master/brainrender/Utils/data_io.py#L215) online

```python
def get_probe_points_from_sharptrack(points_filepath,
    scale_factor=10):
```

   
docstring:

```text
Loads the location of the of probe points as extracted by SharpTrack

[https://github.com/cortex-lab/allenCCF].

:param points_filepath: str, path to a .mat file with probe points

:param scale_factor: 10, sharptrack uses a 10um reference atlas so the

coordinates need to be scaled to match brainrender's
```

