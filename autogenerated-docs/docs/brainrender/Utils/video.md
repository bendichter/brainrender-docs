



Contents
========

* [**`cap_set_frame`** [#15]](#cap_set_frame-15)
* [**`get_cap_selected_frame`** [#22]](#get_cap_selected_frame-22)
* [**`get_video_params`** [#35]](#get_video_params-35)
* [**`open_cvwriter`** [#56]](#open_cvwriter-56)
* [**`save_videocap_to_video`** [#81]](#save_videocap_to_video-81)


&nbsp;

--------
# **`cap_set_frame`** [#15]
  
Check the [***``source code``***](https://github.com/BrancoLab/BrainRender/blob/master/brainrender/Utils/video.py#L15) online

```python
def cap_set_frame(cap, frame_number):
```

&nbsp;  
docstring:

```text
Sets an opencv video capture object to a specific frame

```

&nbsp;

--------
# **`get_cap_selected_frame`** [#22]
  
Check the [***``source code``***](https://github.com/BrancoLab/BrainRender/blob/master/brainrender/Utils/video.py#L22) online

```python
def get_cap_selected_frame(cap, show_frame):
```

&nbsp;  
docstring:

```text
Gets a frame from an opencv video capture object to a specific frame

```

&nbsp;

--------
# **`get_video_params`** [#35]
  
Check the [***``source code``***](https://github.com/BrancoLab/BrainRender/blob/master/brainrender/Utils/video.py#L35) online

```python
def get_video_params(cap):
```

&nbsp;  
docstring:

```text
Gets video parameters from an opencv video capture object

```

&nbsp;

--------
# **`open_cvwriter`** [#56]
  
Check the [***``source code``***](https://github.com/BrancoLab/BrainRender/blob/master/brainrender/Utils/video.py#L56) online

```python
def open_cvwriter(filepath, w=None, h=None, framerate=None,
    format='.mp4', iscolor=False):
```

&nbsp;  
docstring:

```text
Creats an instance of cv.VideoWriter to write frames to video using
    python opencv

:param filepath: str, path to file to save

:param w,h: width and height of frame in pixels

:param framerate: fps of output video

:param format: video format

:param iscolor: bool, set as true if images are rgb, else false if
    they are gray

```

&nbsp;

--------
# **`save_videocap_to_video`** [#81]
  
Check the [***``source code``***](https://github.com/BrancoLab/BrainRender/blob/master/brainrender/Utils/video.py#L81) online

```python
def save_videocap_to_video(cap, savepath, fmt, fps=30, iscolor=True):
```

&nbsp;  
docstring:

```text
Saves the content of a videocapture opencv object to a file

```