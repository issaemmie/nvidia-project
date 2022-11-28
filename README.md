# color detector
  The jupyter lab based color detector allows a person to show an object and receive the color that it is back. For example, this can help people who have color blindness or who have difficulty differing between colors.
 ! color being detected <img width="1116" alt="workingColorDetect" src="https://user-images.githubusercontent.com/99782654/202931547-3f693b24-7442-44b7-a31b-1c72ebb64593.png">
 
## the algorithm
 This project works by first initializing the camera from the jetson nano and importing it in. I added categories of colors (red, orange, yellow, green, blue, and purple) and data into each set. The data was pictures taken of each color that the algorithm then used to process what color the object shown would be. I then trained the model through every batch of photos and increased the accuracy of the model. The quality of the data was important to how well the model could function. For example, if the pictures added had a detailed background, the machine would pick up on those things as well as the object I was trying to capture, making the data muddled. A solution to this is to take pictures with a black or white background and to keep it as consistent as possible across the data sets.

## running this project
For the color detector to work, the jetson inference library is required. To make the project function, run each cell in the jupyter lab code, and make sure that a confirmation prints after each cell. After putting it all together, a menu page will pop up, and simply input a number for epochs to train, 5 is recommended, wait for it to finish, and the model will be ready to detect. Show an object in front of the camera and it will return the color.

## video demonstration
https://youtu.be/zm8Ps2rBVgc
