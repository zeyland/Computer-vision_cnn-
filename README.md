# Computer-vision_cnn-
Improvement Of The Qualıty Control Process By Usıng Computer Vısıon Technology: Lemon Applıcatıon


Dataset
 100 kilograms of lemon fruit to create the dateset
 100 images of each lemon fruit
 When erroneous, low-quality images are extracted from lemon images, 12 different angles of view for each fruit
 2690 annotated images (1056 x 1056 pixels)
 The characteristics of lemons of different quality are categorized as follows: healthy, color (green fruit), sick, gangrene, mold, stained.


######################################
No	Conv2D   Filters	Conv2D activation	MaxPooling2D	Loss	Optimizer	Result
1	32	Relu	  2	     Sparse_categorical_crossentropy	Rmsprop	0.707
2	32	Softmax	2    	 Mse	Rmsprop	0.027
3	32	Sigmoid	2	     Binary_crossentropy	Rmsprop    	0.688
4	64	Sigmoid	2    	 Binary_crossentropy	Rmsprop   	0.715
5	64	Sigmoid	2	     Categorical_crossentropy	Adam	  0.710
6	64	Relu	(2.2)	   Categorical_crossentropy	Adam	  0.709
7	128	Relu	 3	     Categorical_crossentropy	Adam	  0.706
