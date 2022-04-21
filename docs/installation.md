# wgsalign: Installation

The wgsalign pipeline is already installed in myriad. You just need to load it and start using it:

```bash
module load blic-modules
module load nextflow_wgsalign

nextflow_wgsalign --reads '*_R{1,2}.fastq.gz' --genome GRCh38
```

By default, the pipeline runs with the `legion` configuration profile [`conf/legion.config`](../conf/legion.config) if you submit it from legion, and with the `myriad` config [`conf/myriad.config`](../conf/myriad.config) if you send 
the job from myriad.

The 'standard' configuration (using the `local` executor) is not enabled.
