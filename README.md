# Signature to graph 

## Code Structure
This code gets an image of a handwritten signature and converts it into the underlying graph structure of the same signature, which can be used for later classification tasks. This code consists of four modules:

- in the first one, we create a black-and-white image from the given input and turn it into a skeleton image of the signature

- then, using the second module, we construct a graph to represent the underlying pattern of the skeleton image

- the display module, which creates the plots and then shows the output to us

- and lastly, the interface and run module, which allows user to upload images and config the parameters of the program


## Parameters
There are some parameters which one can change and make different outputs. which inputs the following parameters:

- ```output_name``` : The name of file which you want the result saves into. It is not required and has a default value of output.png.

Example : ```output_name='MyFile.png'```

- ```sigma1``` : The sigma value for the first gaussian filter in DoG calculations. It is not required and has a default value of 1.

Example : ```sigma1=2```

- ```sigma2``` : The sigma value for the second gaussian filter in DoG calculations. It is not required and has a default value of 30.

Example : ```sigma2=40```

- ```threshold``` : The threshold for which the color of a pixel will determined to be black or white. It is not required and has a default value of 0.87.

Example : ```threshold=0.4```

- ```h_res``` : The elucidian distance (in pixles) between two adjacent nodes of the result high resolution graph. Note that since we have some nodes for junctions, the distance between a junction node and a normal node can be lower ! It is not required and has a default value of 10.

Example : ```h_res=20```

- ```m_res``` : The elucidian distance (in pixles) between two adjacent nodes of the result mid resolution graph. Note that since we have some nodes for junctions, the distance between a junction node and a normal node can be lower ! It is not required and has a default value of 40.

Example : ```m_res=80```

- ```l_res``` : The elucidian distance (in pixles) between two adjacent nodes of the result low resolution graph. Note that since we have some nodes for junctions, the distance between a junction node and a normal node can be lower ! It is not required and has a default value of 80.

Example : ```l_res=120```


## References 
The original owner of this code is @DIVA-DIA and this code is a compact version of the same code which can be executed in colab. The link to their repository is here : ```https://github.com/DIVA-DIA/SkeletonGraph```
