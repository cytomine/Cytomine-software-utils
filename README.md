# Cytomine software utils
You will find here all the Dockerfiles used to compile the docker images of the Cytomine clients.
These images are used in the Cytomine external softwares. See our [documentation](https://doc.cytomine.org/DataScientists) to know how to create your own script or software to interact with a Cytomine instance.


## How to compile it
You will find below a script to compile all the images.
      
    cd software-groovy2-4-base && docker build -t cytomine/software-groovy-2-4-base:v2.0.0 .
    cd ../software-java8-base && docker build -t cytomine/software-java8-base:v2.1.0 .
    cd ../software-python2-base && docker build -t cytomine/software-python2-base:v2.2.0 .
    cd ../software-python3-base && docker build -t cytomine/software-python3-base:v2.2.0 .
    cd ..
    echo DONE
