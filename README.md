-	Our source code link is a kaggle notebook : https://www.kaggle.com/code/kawwie/neural-style-transfer

-	In the "Initialize images" cell: 

The user need to set the base_img_link and the style_img_link, which is the link to the content and style images respectively
The user need to set their desired img_height and img_width, both of them should be even numbers to avoid the image transform net's output being in the wrong dimension

-	To train an image transform net :
Run the "Training image transform net" cell, the user can specify total_variation_weight, style_weight, content_weight, number of epochs to be used
We are training the model on the COCO 2017 image dataset

-	To transfer style using our pretrained network on the "starry skies" style image:
Run the "Style transfer using our pretrained image transform net" cell

-	To apply style to base image directly :
Run the "Apply style directly on image" cell, the user can specify total_variation_weight, style_weight, content_weight and number of iterations to optimize the image for
The system will save output after every 100 iterations in the "kaggle/working" folder

-	To visualize our image tranform network architecture:
Run visualize_model()
