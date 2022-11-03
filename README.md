# Cochran

The legal document scoring model

<img src="./docs/Cochran.jpeg" alt="Cochran Logo"/>


# TODOs 

* [API Official](https://www.courtlistener.com/api/rest-info/)
* [API Guide/Blog](https://github.com/tedrand/claimkraken-netlify-cms/blob/57cc7e7d768ccbe7de09c7476c8ba58ff79e31d2/src/pages/blog/2021-08-09-tracking-cafc-opinions-with-courtlistener-and-python-part-1.md)
* Connect to API and make downloader, experiment with courts
* [Brazil?](https://huggingface.co/datasets/joelito/brazilian_court_decisions)

# Data Sources

* [Court Listener](https://www.courtlistener.com/api/bulk-info/)
* [US Court Records](https://www.uscourts.gov/court-records)
* [Federal Court Cases](https://www.icpsr.umich.edu/web/NACJD/series/72)
* [Justice.gov](https://www.justice.gov/jmd/ls/state)
* [Justia](https://dockets.justia.com/)
* [Federal Records Center](https://www.archives.gov/frc/atlanta)
* [Supreme Court](https://www.supremecourt.gov/docket/docket.aspx)
* [UCLA Law Library](https://libguides.law.ucla.edu/dockets/federal)
* [VA Courts]( https://www.vacourts.gov/courtadmin/library/federal.html)
* [Data.gov](https://data.gov)


# Requirements

* [docker](https://www.docker.com/)
* a bash shell

# Getting Started

* start your training environment by running ```sh run-training-environment.sh``` or ```sh gpu-environment.sh``` and follow the link to the jupyter server
* Use a [downloader](./downloader/) to download a dataset into the [data](./data/) folder
* Run a [training notebook](./training_notebooks) to fit your model
* Export your model to the [saved models](./saved_models) folder
* Shrink, optimize, and deploy your model, see [deploy](./deploy) for examples 

# Frequently Asked Questions

### Will this run on Windows or macOS?

Yes, but you need to install docker first, see link above. if on Windows run the ```windows-training-environment.sh``` feel free to open an issue if that doesn't work. 

### How to I shut down the notebook?

Go to the terminal where you ran the ```run-training....sh``` and press ```CTRL+C```, [WTF](https://medium.com/@aantipov/what-happens-when-you-ctrl-c-in-the-terminal-36b093443e06)

### What the hell is this notebook stuff?

Try this tutorial to learn more [tutorial](https://jupyter.org/try)

### Can I deploy this in a cloud environment via Docker? or run it on my big ML rig with many nvidia GPUs?

Hell yes you can! I'll eventually write a more detailed guide here on how to do that, but the setup is almost identical to running locally.
