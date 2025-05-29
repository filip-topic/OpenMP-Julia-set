Parallelized implementation of Julia set implementation is in ./src/juliap.c

Parallelized implementation of gaussian filter is in ./src/filter.c

Project needs to be uploaded to the cluster in the ./project folder as .tar.bz2
then run:

tar xfvj julia-student-1.0.0-Source.tar.bz2
cd julia-student-1.0.0-Source/
cmake .
make
sbatch run_juliap.job
sbatch run_juliap2.job
sbatch run_filter_strong.job
sbatch run_filter_weak.job
