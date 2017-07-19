FROM opencpu/rstudio


RUN add-apt-repository -y ppa:ubuntugis/ppa && \
    apt-get update && \
    apt-get install -y \
    lbzip2 \
    libdap-dev \
    libexpat1-dev \
    libfftw3-dev \
    libfreexl-dev \
    libgdal-dev \
    libgeos-dev \
    libgsl0-dev \
    libglu1-mesa-dev \
    libhdf4-alt-dev \
    libhdf5-dev \
    liblwgeom-dev \
    libkml-dev \
    libnetcdf-dev \
    libproj-dev \
    libsqlite3-dev \
    libssl-dev \
    libtcl8.5 \
    libtk8.5 \
    libtiff5-dev \
    libudunits2-dev \
    libv8-dev \
    libxerces-c-dev \
    netcdf-bin \
    unixodbc-dev


## Install R packages

RUN Rscript -e "install.packages(c( \
'deldir', \
'DCluster', \
'classInt', \
'fastcluster', \
'geojsonio', \
'geoR', \
'geosphere', \
'gstat', \
'igraph', \
'lidR', \
'leaflet', \
'maptools', \
'ncdf4', \
'proj4', \
'postGIStools', \
'rasterVis', \
'raster', \
'rgdal', \
'rgeos', \
'rlas', \
'rmapshaper', \
'roxygen2', \
'RandomFields', \
'RColorBrewer', \
'RSQLite', \
'RMySQL', \
'sf', \
'sp', \
'spacetime', \
'spatstat', \
'spdep', \
'splancs', \
'testthat', \
'tidyverse' \
), repos='https://cran.r-project.org/'); \
source('https://bioconductor.org/biocLite.R'); \
biocLite('BiocInstaller'); \
BiocInstaller::biocLite('rhdf5')"




