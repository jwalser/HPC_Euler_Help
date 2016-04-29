## Job - Arrays

A simplest case for a job array:

```bash
bsub -J "test[1-4]" "echo \$LSB_JOBINDEX"
```


$TMPDIR is a directory on the local hard drive, which LSF creates for each job. 
