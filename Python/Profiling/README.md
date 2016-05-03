# Profiling
The Python standard library offers the cProfile module, which can be used
to determine the functions that use most compute time.

The `line_profiler` gives more detailed information, but incurs substantial
overhead.  Hence it is best to use it only to profile the single function
the optimization process is currently focussing on.

## What is it?
1. `primes_cprof.py`: Python script to profile using `cProfile`.
1. `primes_lprof.py`: Python script to profile using `line_profiler`.
1. `run_cprofile.sh`: Bash shell script to run the `cProfile`.
1. `run_kernprof.sh`: Bash shell script to run the `kernprof`
    `line_profiler`).
1. `run_snakeviz.sh`: Bash shell script to to `cProfile`, save the profile
    to a file and invoke `snakeviz` to visualize it.