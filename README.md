# PIGMMaLIOnde
Adapting Gaussian Mixture Model Training to Embedded/Edge Devices: a Low I/O, Deadline-aware and energy efficient Design

#download the github repo #download armadillo libarary on ubuntu distribution:

sudo apt-get install liblapack-dev

sudo apt-get install libblas-dev

sudo apt-get install libboost-dev

sudo apt-get install libarmadillo-dev

check site for more info: https://www.uio.no/studier/emner/matnat/fys/FYS4411/v13/guides/installing-armadillo/

#Replace the files gmm_diag_bones and gmm_diag_meat of the armadillo source code:

sudo cp gmm_diag_bones /usr/include/armadillo_bits/gmm_diag_bones

sudo cp gmm_diag_meat /usr/include/armadillo_bits/gmm_diag_meat

#create folder data inside the repo and put your dataset in

g++ main.cpp -o main -larmadillo -llapack -lblas

set linux governor to userspace to control frequencies

sudo ./main nb_increments #where nb_increments=size_data_set/size_available_memory. 


