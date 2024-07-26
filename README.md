# almost-infinite-sites-recursions
Joint work with A. Avalos-Pacheco. Plublically availiable coppy of python-implementation of almost-inifinite-sites-recursions.

To generate likelihood curves, install required external libraries (numpy, matplotlib), and run

```{python}
python generate_MLE_Likelihood.py input_file_path output_dir [n_cores = 4] [b = 1]
```
The **input_file_path** should be a .csv file encoding a configuration (see inline documentation of csv2psi.py for details of how to encode configurations as .csv files).

The **output_dir** should be the path where you want your output saved. The script will generate .png, .pdf, .jpg, and .eps renderings of the likelihood curve(s), along with the raw .csv data of all tickpoints in the figure which can be used as input for other plotting tools if desired.

the **n_cores** arguments indicates how many cores should be employed when doing calculations. Default value is 4.

all arguments after the first 3 are considered different b-values, so if multiple likelihood curves are desired with different b-values in the same figure, call the script with more than 4 arguments.
