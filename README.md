# SWEGrapher
This is a a MLP for predicting SWE based on SNOTEL data, courtesy of Liza Gunther and Kevin Lane!  

You can programmatically generate a .csv file of relevent SNOTEL data based on our snotel_download_data notebook.

The snotel-mlp(4) r2 > 0.95 notebook contains our code for an initial vanilla mlp, and should serve as a good starting point for understanding the data.

Our swe-grapher notebook contains the same mlp, but with a number of changes designed to work with our long-tail data distribution, including:
- Upsampling (with a ceiling configuration)
- Downsampling
- Stratified testing
- Variable size binning for stratification
