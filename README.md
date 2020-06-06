# Linux Mint
This is a brief introduction how to get started with Linux Mint for data science and academic research. 


## Install R
Install R via the terminal:
> sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
> sudo add-apt-repository 'deb https://cloud.r-project.org/bin/linux/ubuntu bionic-cran35/'
> sudo apt update
> sudo apt-get install r-base

You can test R by simply: 
> R
> install.packages("ggplot2")
> q()

## Install Rstudio
get the name of the last Ubuntu/Debian Rstudio version at https://rstudio.com/products/rstudio/download/#download
> wget https://download1.rstudio.org/desktop/bionic/amd64/rstudio-1.3.959-amd64.deb
If needed to install gdebi:
> sudo apt install gdebi
Then install the deb-file:
> sudo gdebi rstudio-1.3.959-amd64.deb

## Install Gitkraken
This can be done via the software manager or via: 
> wget https://release.gitkraken.com/linux/gitkraken-amd64.tar.gz
> sudo tar -xvzf gitkraken-amd64.tar.g

## Repair broken packages
Not all goes perfect the first time, so in case something brakes down:
> sudo apt update --fix-missing
> sudo apt install -f
