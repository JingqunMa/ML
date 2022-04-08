# ML
Apply machine learning algorithm and artificial intelligence methods for precision medicine

4/8 initial successful run with tensorflow2
1. encountered issue when running on HPC cloud, used docker tensorflow image instead. In order to access the my data, need to run image with 
docker run -v mylocal:/tf -it -p 8888:8888 tensorflow/tensorflow:latest-jupyter     
2. since this image doesn't have pandas and numpy, need to run following to install those successfully: 
	Docker exec CONAINER_name pip3 install pandas, numpy
Commit the docker container for next use. 
	Docker commit CONAINER_name new_container_name

