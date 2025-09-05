# Prerequisites

Run the following command to install the Python packages that are required to run the jupyter notebooks

```console
pip install notebook matplotlib numpy opencv-python Pillow msl-kcdb
```

Converting the AVI videos to the MP4 format uses the [ffmpeg](https://ffmpeg.org/download.html) tool. The `ffmpeg` executable must be available on your `PATH` environment variable. To test that the `ffmpeg` executable is installed properly, run `ffmpeg -version` and you should see information about the `ffmpeg` tool &dash; such as the version number, how `ffmpeg` was built and the configuration settings.

# Run the notebooks

To start the jupyter server, run

```console
jupyter notebook
```

The notebooks do not create the _SI reference point_ data that should be made available at `input/kcdb_data_output_physics.txt`. This file must be acquired another way. It is required by `Extract CMCs with years.ipynb`.

The execution order of the notebooks to re-generate the videos for the website and the images for the report is

1. physics-non-zero-cmc.ipynb
2. Extract CMCs with years.ipynb
3. Create Boxplots.ipynb
4. Create Videos.ipynb
5. convert-avi-to-mp4.ipynb
