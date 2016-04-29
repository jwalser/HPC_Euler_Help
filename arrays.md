### Job - Arrays

There are times when users need to execute the same script multiple times for different input files. Of course you can submit multiple jobs individually but depending on the number of submission this could be tedious. The HPC scheduler provides solutions and "Job Arrays" is one of them. Here is a howto to get you started an explore the possibilities of a job array on Euler. 

A simplest case for a job array:

```bash
bsub -J "test[1-4]" "echo \$LSB_JOBINDEX"
```



$LSB_JOBINDEX


$TMPDIR is a directory on the local hard drive, which LSF creates for each job. 
