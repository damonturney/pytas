# pytas
Python for transient absorption spectroscopy: a suite of GUI tools based on matplotlib and QT.


# Installation
conda install -c conda-forge pytas
or
mamba install -c conda-forge pytas


# List of included GUI applications

TA_plot_matrix_GUI                    

TA_t0_correction_and_background_removal_GUI

TA_merge_matrices_GUI               



# List of included Supporting Functions
TA_matrix_window_average(TA_matrix,window_size)

create_TA_Blue_White_Red_colormap(min_max)

create_TA_Blue_White_Red_Black_colormap(min_max)

list_hdf5_contents(HDF5_filename)

load_hdf5_data(filename,dataset_path_string)



# Input File Compatibility
Presently just .h5 or .hdf5 or .hdf


# Example Work Flows
To run the GUI applications from a terminal shell:
python -m pytas.TA_plot_matrix_GUI data.h5
python -m pytas.TA_t0_correction_and_background_removal_GUI data.h5
python -m pytas.TA_merge_matrices_GUI data1.h5 data2.h5

or from a python REPL (e.g. from python or ipython or Jupyter Notebook or Spyder):
import pytas
data_filename1 = 'data1.h5'
pytas.pytas.TA_plot_matrix_GUI(data_filename1)
pytas.pytas.TA_t0_correction_and_background_removal_GUI(data_filename1)
data_filename2 = 'data2.h5'
pytas.pytas.TA_merge_matrices_GUI(data_filename1, data_filename2)



# Next Code To Develop
SVD amd Global Analysis module 



# Home Repository
https://github.com/damonturney/pytas


