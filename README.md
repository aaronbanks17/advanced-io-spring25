# Avanced IO Homework

Homework assignments from 14.273 - Advanced Topics in Industrial Organization

## Setup and Installation (Unix Systems Only)
The following provides the steps to get the code and data setup on your local machine. The instructions are for Unix-based systems (MacOS, Linux). 

1) Clone the repository to a private directory (not shared on dropbox)
```bash
mkdir advanced-io
git clone git@github.com:aaronbanks17/advanced-io-spring25.git ./advanced-io/code
```
2) Symlink the `data` directory from the shared Dropbox folder to the top level of the repository
```bash
ln -s "/path/to/Dropbox/folder/data/" ./advanced-io/data
```
3) Install mamba if not already installed
```bash
# On Mac
# Install homebrew if you don't have it
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# Then install miniforge
brew install miniforge

# on Linux
curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
```
4) Create the mamba environment
```bash
# Cd into the code directory if you are not already there
cd advanced-io/code
# create the environment
mamba env create --name advanced_io --file AdvancedIO.yaml
```
5) Activate the environment
```bash
mamba activate mergers
```