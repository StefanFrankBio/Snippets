### Search for all available package verions in conda channel:
```
conda search -c example_channel -f example_package
```   
### Update conda in the base environment:
```
conda update -n base -c defaults conda
```
### Create a conda environment from .yml file:
```
conda env create -f example.yml
```
### Remove a conda environment:
```
conda env remove -n example_name
```
### Remove unused packages:
```
conda clean --all
```
### Structure of conda environment.yml file:
```yml
name: example_name

channels:
  - example_channel_1
  - example_channel_2

dependencies:
  - example_package_1=1.0.5
  - example_package_2=1.1.3
  - example_package_2=3.0.5
``` 
### Uninstall conda:
```
conda activate base
conda install anaconda-clean
anaconda-clean --yes
rm -rf path/to/miniconda3
rm -rf ~/.anaconda_backup
```
### Create executable bash script:
```bash
#!/bin/bash
chmod +x myscript.sh
```
### Redirect stdout and stderr to the same file:
```bash
command > log.txt 2>&1
```
### Redirect stdout and stderr to different files:
```bash
command > stdout.log 2> stderr.log
```
### Get the size of a file or directory:
```bash
du -sh example_file
```
### Delete all empty files and directories:
```bash
find . -type f -empty -delete -o -type d -empty -delete
```
