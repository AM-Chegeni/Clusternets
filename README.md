# k-Nets
## A deep learning approach for distinguishing ΛCDM and k-essence cosmologies

This is a code related to the article titled "A deep learning approach for distinguishing ΛCDM and k-essence cosmologies". In this paper, we employ two ML algorithms to study the capability of ML in distinguishing k-essence type theories from the Lambda Cold Dark Matter (ΛCDM) ones. We train the Convolutional Neural Network (CNN) algorithm over the randomly chosen density patches of N -body simulation snapshots from gevolution and k-evolution codes. Our results show that the CNN algorithm is a powerful tool to distinguish k-essence theories even in case the matter power spectra of these theories are barely distinguishable. The accuracy of the CNN algorithm can be improved by 10-20% compared to the Random Forest (RF) algorithm trained over the power spectra. We find that the CNN algorithm has higher accuracy in small scales relative to the RF algorithm. Our strategy to use random patches of simulations for training the CNN algorithm, can be a useful tool to distinguish k-essence and ΛCDM cosmologies from a random patch of the sky.

## User manual

First, adjust your parameter in config.ini file:

* main_box = The Number of Ngrid in simulation snapshots ( 128 or 256)

* sub_box =  The Number of Ngrid in sub-boxes seperate from the main boxes (16, 32, 64, 12)
* Number_of_sub_boxes: The number of seperated sub-boxes
* ml_algorithm: The algorithm that use to train machine. It can be CNN, RF, or both of them (cnn,rf or both)
* boxsize: The size of boxes in simulation snapshots 

* path_LCDM_X = The path of 6 Gadget ΛCDM simulation snapshots 
* path_k_X = The path of 6 Gadget k-essence simulation snapshots 

Then run the run.sh in terminal and get the results!
