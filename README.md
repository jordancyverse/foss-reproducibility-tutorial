# Foss Reproducibility Tutorial
    1  cd /scratch/
    2  /opt/conda/bin/conda search -c bioconda snakemake
    3  /opt/conda/bin/conda install -c bioconda -c conda-forge -y snakemake=5.8.1
    4  ln -s /opt/conda/bin/* /bin
    5  ln -s /opt/conda/lib/* /usr/lib
    6  snakemake --version
    7  sudo apt-get update
    8  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
    9  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   10  sudo add-apt-repository  "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
   11  sudo apt-get update
   12  sudo apt-get install -y docker-ce docker-ce-cli containerd.io
   13  docker run hello-world
