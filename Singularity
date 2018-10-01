Bootstrap: docker
From: ubuntu:latest

%files 
NAMD_2.13b1_Linux-x86_64-multicore.tar.gz /opt

%post
apt-get update
apt-get install -y vim 
cd /opt
tar -xzvf NAMD_2.13b1_Linux-x86_64-multicore.tar.gz

echo 'export PATH=/opt/NAMD_2.13b1_Linux-x86_64-multicore:$PATH' >>$SINGULARITY_ENVIRONMENT

% environment
export PATH=/opt/NAMD_2.13b1_Linux-x86_64-multicore:$PATH
