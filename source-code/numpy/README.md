# Numpy

Numpy is the de facto standard for efficient matrix representations and
(BLAS level 1-3) computations.  Scipy implements more high-level
algorithms for scientific computing (Lapack, statistics,...).


## What is it?

1. `data_plot.py`: reads a CSV file containing data, performs linear
    regression, and plots the data and the line representing the regression;
    numpy is used to represent the data, scipy to perform the linear
    regression, matplotlib for plotting the result
1. `data_writer.py`: produces data for the `data_plot.py` script, linear
    with noise added
1. `data.csv`: example data set for `data_plot.py`
1. `diffusion.ipynb`: solving the PDE describing thermal diffusion in 2D.
1. `fft.py`: creates a signal consisting of a sum of cosine functions
    with specified amplitudes and frequencies, adding noise; plots the
    resulting function, uses FFT to determine the frequency spectrum, and
    plot the latter
1. `fft_experiments.ipynb`: notebook with some experiments on signal
    analysis using FFT.
1. `game_of_life.ipynb`: jupyter notebook implementing Game of Life.
1. `logistic_map.ipynb`: analysis and visualization of the logistic map.
1. `numeexpr.ipynb`: Jupyter notebook illustrating some use cases of the
    numexpr module.
1. `numpy.ipynb`: Jupyter notebook illustrating some numpy aspects like
    array slicing, adding dimension to arrays, and so on.
1. `optimization.py`: illustration of how to use the `scipy.optimize` for
    unconstrained multivariate optimization
1. `target_function_plot.py`: script that creates a surface plot of the
    target function in `optimization.py`
1. `pendulum_ode.py`: solves the ODE of a damped, driven pendulum that is
    optionally anharmonic. Optionally plots results.
1. `dynamic_programming.ipynb`: example of string alignment using
    dynamic programming.
1. `vector_write.py`: script to create a file containing a specified number
    of floating point values, either in text or binary format to test I/O
    performance characteristics.
1. `vector_sum.py`: reads files generated by `vector_write.py` and computes
    the sum of the values; intended for I/O performance tests.


## Pendulum

For chaotic regime, choose the following parameters:
  * `l = 9.81`
  * `q = 0.5`
  * `F_d = 1.2`
  * `omega_d = 0.66667` (2/3)
  * `theta0 = 0.2`
  * `anharmonic`

To easily obtain as many points as possible for the Poicare section, choose
`delta_t ~ 3pi`, e.g., `delta_t = 0.009424778`.