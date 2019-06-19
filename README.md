# CMDprior
These jupyter notebooks lay out how to simply generate Galaxy priors using the [GDR2mock](http://adsabs.harvard.edu/abs/2018PASP..130g4101R) catalogue and they can also help to get a quick interface with the [isochrones](https://github.com/timothydmorton/isochrones) and [brutus](https://github.com/joshspeagle/brutus) isochrone fitting packages.

# Running the jupyter notebooks
In order to run those jupyter notebooks on your local machine you will need to install a few necessary packages. You will also need some additional data in the data folder in order to run the brutus package. If you do not want to run the ADQL-TAP queries yourself, you can download the GDR2mock samples used in the notebooks together with the brutus data from [here](https://keeper.mpdl.mpg.de/d/51feb58454a5450f9cf4/).

# Example science case
In particular they were used in the following science paper: Arxiv reference

# Description of individual files

  - HD*.fits are the GDR2 data of the respective stars
  - [GDR2mock_prior_query.ipynb](https://github.com/jan-rybizki/CMDprior/blob/master/GDR2mock_prior_query.ipynb): Example GDR2mock prior query of the 130pc sample
  - [GDR2mock_prior_masses.ipynb](https://github.com/jan-rybizki/CMDprior/blob/master/GDR2mock_prior_masses.ipynb): The CMDprior using the 130pc sample applied to our 3 planetary hosts.
  - [HRD selection dereddened.ipynb](https://github.com/jan-rybizki/CMDprior/blob/master/HRD%20selection%20dereddened.ipynb):
  An example query to query all stars in GDR2mock with specific absolute magnitude and BP-RP range, as used for HD 33142.
  - [Masses for HD33142 HD76700 HD205739.ipynb](https://github.com/jan-rybizki/CMDprior/blob/master/Masses%20for%20HD33142%20HD76700%20HD205739.ipynb): Using the [isochrones](https://github.com/timothydmorton/isochrones) package to infer the stellar parameters, also including a query to [mwdust](https://github.com/jobovy/mwdust) to get an idea of the extinction prior.
  - [Inference_with_brutus.ipynb](https://github.com/jan-rybizki/CMDprior/blob/master/Inference_with_brutus.ipynb): Same inference now using the [brutus](https://github.com/joshspeagle/brutus) package

# Attribution
If you use those notebooks in your science please cite: ASCL reference

Also cite the relevant packages and catalogues used.

![](data/CMDcover.png)
CMD prior for the planetary host stars from the paper. This shows the CMD of all stars within 130 pc in GDR2mock catalogue.
