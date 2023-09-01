This repository contains the code and data for the project. Below is an overview of the files and their purposes:

## Files

### benchmark_and_noise.ipynb

This file generates exhaustive synthetic datasets. Each dataset consists of a three-feature dataset, where features are set to highly correlate in spatial context. The datasets are generated using a realistic application of unconditional Sequential Gaussian Simulation. These datasets are then exposed to different levels of noise: a base case with 0% noise, and 10%, 20%, and 30% noise levels. The percentage indicates the amount of variance contributed by the added Gaussian noise.

### var_reader.ipynb

This file is used to check and read variograms. From this step, the experiment is carried out, resulting in having half of the data and only the 5th grid samplings available. The truth model will not be available from this point onward.

### main_loop.ipynb

This is the main loop for the experiment. It involves finding the number of effective sample size and hyperparameter tuning for dense intervals of sample sizes from 2 to n_standard_bootstrap. The experimentation is done extensively for each unique dataset, and the results are compiled in accompanying .json files.

### plotter_eda.ipynb

This file contains plotting code for exploratory data analysis used in the paper. It helps in visualizing and understanding the characteristics of the datasets.

### plot_results.ipynb

This file contains plotting code to visualize the compiled results presented in the paper. The results from the main loop are visualized in various plots to showcase the outcomes of the experiment.

## Usage

To use these files, follow the steps outlined in each notebook. Each notebook is designed to perform specific tasks and contribute to the overall project's objectives.

Feel free to explore and adapt the code as needed for your own analysis and experimentation.

For any questions or inquiries, please contact [fehmi@utexas.edu].


