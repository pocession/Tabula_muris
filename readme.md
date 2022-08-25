# Tabula_muris_LargeIntestine: a project for identifying aging-related biomarkers in large intestine
Large intestine is the largest habitat for microbiota as well as the largest immune tissues. To help people understand how aging affect the large intestine physiology, I collect and visualize the Tabula muris data.

## How I get and process the data
1. The data was first downloaded from Tabula muris senis [10X](s3://czb-tabula-muris-senis/Data-objects/tabula-muris-senis-droplet-processed-official-annotations.h5ad) and [SMARTseq](s3://czb-tabula-muris-senis/Data-objects/tabula-muris-senis-facs-processed-official-annotations.h5ad).
2. The downloaded h5ad files then were processed by [my phton script](scRNA_differentialAnalysis.ipynb)
3. The main toolkit is [scanpy](https://scanpy.readthedocs.io/en/stable/).
4. The IDE is [Visual Studio code](https://code.visualstudio.com/).

## The files are organized as the following structure
```
github.com/pocession/Tabula_muris/
├── subset: csv files for subsetted data
│   ├── *.csv
├── figures : pdf or png files for output data
│   ├── *.pdf
|   ├── *.png
├── output : csv files for output data, used by Tableau
│   ├── *.csv
├── scRNA_differentialAnalysis.ipynb: the python script for processing the input data
├── SscRNA_subsetting.ipynb: the python script for subsetting the original data
├── readme.md
├── *.h5ad: original h5ad files
```

The processed data is provided in 'csv' formats and stored in the follwoing folder, `output`.

## Useful links
- [Data source](https://s3.console.aws.amazon.com/s3/buckets/czb-tabula-muris-senis?region=us-west-2&tab=objects)
- [Tabula muris project](https://tabula-muris.ds.czbiohub.org/)
- [Tabula muris github](https://github.com/czbiohub/tabula-muris)
- [scanpy](https://scanpy.readthedocs.io/en/stable/)
- [Tableau](https://public.tableau.com/app/profile/tsunghan.hsieh/viz/covid19_16606524256070/1)
