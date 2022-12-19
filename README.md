# Conda
### Search for all available package verions in conda channel:
```conda
conda search -c example_channel -f example_package
```   
### Update conda in the base environment:
    conda update -n base -c defaults conda

### Create a conda environment from .yml file:
    conda env create -f example.yml
    
### Structure of conda environemtn .yml file:
    name: example_name

    channels:
      - example_channel_1
      - example_channel_2

    dependencies:
        - example_package_1=1.0.5
        - example_package_2=1.1.3
        - example_package_2=3.0.5
