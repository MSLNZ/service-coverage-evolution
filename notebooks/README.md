# Prerequisites

Run the following command to install the Python packages that are required to run the jupyter notebooks

```console
pip install notebook matplotlib numpy opencv-python Pillow msl-kcdb
```

Converting the AVI videos to the MP4 format uses the [ffmpeg](https://ffmpeg.org/download.html) tool. The `ffmpeg` executable must be available on your `PATH` environment variable. To test that the `ffmpeg` executable is installed properly, run `ffmpeg -version` and you should see information about the `ffmpeg` tool &mdash; such as the version number, how `ffmpeg` was built and the configuration settings.

# Run the notebooks

To start the jupyter server, run

```console
jupyter notebook
```

> [!IMPORTANT]
> The notebooks do not create the _SI reference point_ data that must be saved to `input\kcdb_data_output_physics.txt`. This file must be acquired another way. See the [report](https://github.com/MSLNZ/service-coverage-evolution/blob/main/report/report.pdf) for more details. It is required by the `Extract CMCs with years.ipynb` notebook.

The execution order to run the notebooks to regenerate the videos for the website and some of the images for the report is

1. physics-non-zero-cmc.ipynb
2. Extract CMCs with years.ipynb
3. Create Boxplots.ipynb
4. Create Videos.ipynb
5. convert-avi-to-mp4.ipynb
