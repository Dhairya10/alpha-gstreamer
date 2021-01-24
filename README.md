# GStreamer Assignment

## Assignment 1

**Use videotestsrc and get output of 720p resolution**

```
gst-launch-1.0 videotestsrc ! videoconvert ! videoscale ! capsfilter caps="video/x-raw, width=1280, height=720" ! autovideosink
```

## Assignment 2

**Demonstrate audio visualization in GStreamer. Take any audio file and generate any visualization of your choice.**

* cd into Assignment2 directory
* Run the following command 
    ``` 
    gcc audio_visualisation.c -o audio_visualisation `pkg-config --cflags --libs gstreamer-1.0`
    ```
* Run `./audio_visualisation `

Choose a visualisation element from the following.
```
1. Synaescope 
2. GOOM 
3. Monoscope
4. Stereo visualizer
```

## Assignment 3

**Python code to retrieve and display rtsp stream**

* cd into Assignment3 directory
* Populate `self.camlink` field in `main.py`
* Run `python3 main.py`