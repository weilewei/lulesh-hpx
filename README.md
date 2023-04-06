# lulesh-hpx

LULESH 2.0, parallel algorithms version, ported by Weile Wei 
(WeileWei@lbl.gov) from the original version of LULESH found at
https://computing.llnl.gov/projects/co-design/lulesh

## Build

```bash
mkdir build && cd build
cmake \ 
    -DHPX_DIR=/$HOME/install/hpx_Release/lib64/cmake/HPX/ 
    -DCMAKE_BUILD_TYPE=Release .

    ..
```

## Run

```bash
./lulesh2.0 -s 150 --hpx::threads=$NTHREADS
```

where

"-p" prints intermediary results

"-s" defines the size of the problem to use.  For benchmarking, a size
	of 150 is typically used but can be changed to suit the need.
