- We shall experiment with the toy dataset called CIFAR 10, consisting of 60,000 images, of 10 varieties
  like cat,dog,car,truck etc.
#### On how Nearest neighbour classification work
- We put the our_image which we want to find which class it is.
- The image is compared with each and every training image
- The image which is most similar to our_image will be taken, and our_image will retain the name of image.
##### How do we compare two images
- Each image is compared with our_image pixel by pixel, add up all the differences and the image with
  least difference will be taken.
- In other words, given two images and representing them as vectors **I1** and **I2**, We take L1
  distance between them. \n
                                      d1(I1,I2)=∑p|Ip1−Ip2|
