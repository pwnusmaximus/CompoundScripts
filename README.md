# ORCA Compound Scripts Exchange

Welcome to the repository for ORCA compound scripts!

The purpose of this repository is twofold:

1. Provide a curated set of compound scripts from the ORCA developers.
2. Provide a unique location where user-provided compound scripts can be shared.

In particular, if you are publishing papers based on ORCA workflows using the compound script feature, this is a place to store your ‘supporting information.’ In such a case, please also reference the paper in the compound script.


## What are compound scripts?

Compound scripts allow the user to automate complicated workflows directly within the ORCA quantum chemistry software package. It provides direct, easy access to internal results such as energies, frequencies, … No more parsing!

Also, a complicated workflow can be run in a single computation---no need to wait for finished jobs and resubmissions.

## Special Formatting and file extention note
1. While the extention of your input files can be anything, It's recommedned to keep them to the traditional ".inp" (input) or ".cmp" (compound) extentions.
2. While not shown in any of the following examples, a compound script REQUIRES the `%Compound` block to come before any variables. Additionally, if you desire your job to be multi-threaded you will need the `%maxcore` and `%Pal NPROCSHARED` blocks to be above the `%Compound` block
3. Note the `%maxcore` and `%Pal NPROCSHARED` blocks can only be supplied once. All subsequent New_Step sections will re-use the same memory and number of CPUs. 

## How do I contribute?

If you want to share your work, please do so! Keep in mind that your script will be published under the [MIT license](LICENSE), and that you must have the rights to share.

The actual sharing process is simple: Fork the repository and create a pull request. Or just head over to the [ORCA forum][1] and let us help you there!


## What is ORCA?

ORCA is a software package for fast and efficient quantum chemical calculations, developed by Frank Neese and many more. Check it out at the [ORCA forum][1] (it’s free for academic use)!

[1]: https://orcaforum.kofo.mpg.de
