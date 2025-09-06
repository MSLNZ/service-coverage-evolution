Quantifying evolution of service coverage for CIPM MRA participants.

The website to visualise the results is available [here](https://mslnz.github.io/service-coverage-evolution/).

### Overview

* `notebooks/` &mdash; Contains the jupyter notebooks that are used to process KCDB data. The notebooks make the videos for the website and some of the images for the report.
* `report/` &mdash; Contains the documents to generate the report.
* `videos/` &mdash; Contains the videos for the website.
* `index.html` &mdash; The file that is used by GitHub Pages for the website. This file loads the videos that are in the repository on GitHub. If you want to use the files on your local computer (for testing purposes when adding results for another year by re-running the notebooks) open the `index.html` file and search for the text `src`. There are two locations in the file where you can choose whether to load the videos from the local `videos` folder or remotely from the GitHub repository. Comments have been added to the `index.html` file to help identify these locations to edit.
