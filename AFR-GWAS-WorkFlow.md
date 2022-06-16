// For execution on a SLURM scheduler, no containerization.

slurm {
process.executor = 'slurm'
process.queue = queue }

slurmSingularity {
singularity.cacheDir = "${HOME}/project/trampush_325/singularity-cachedir"
process.executor = 'slurm'
singularity.autoMounts = true
singularity.enabled = true
singularity.runOption = "--cleanenv" process.queue = queue }

singularity {
singularity.cacheDir = "${HOME}/project/trampush_325/singularity-cachedir"
singularity.autoMounts = true
singularity.enabled = true }
