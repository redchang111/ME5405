# ME5405
**NUS ME5405 Module - Machine Vision**

Images 1 and 2 are 64x64, 32 level images. These images are shown as coded arrays that contains an alphanumeric character for each pixel. The range of these characters is 0-9 and A-V, which corresponds to 32 levels of gray.

Image 1: Chromosomes (chromo.txt)
For Chromosome Image1 ```(chromo.txt)```, the main function file is chromo.m

```javascript
function greeting(name) {
  console.log(`Hello, ${name}!`);
}

greeting('ChatGPT');
```
Perform the following tasks:

Display the original image on screen.

Threshold the image and convert it into binary image.
Determine an one-pixel thin image of the objects.
Determine the outline(s).
Label the different objects. Discuss and compare 4-connectivity and 8-connectivity in your report.
Image 2: Characters (charact1.txt)

Perform the following tasks:

Display the original image on screen.
Create a binary image using thresholding.
Determine a one-pixel thin image of the characters.
Determine the outline(s) of characters of the image.
Segment the image to separate and label the different characters.
Arrange the characters in one line with the sequence: AB123C
Rotate the output image from Step 6 about its center by 30 degrees.
Using the training dataset (p_dataset_26.zip), train the (conventional) unsupervised classification method of your choice (Here k-nearest neighbors (kNN) is used) to recognize the 6 characters (“1”, “2”, “3”, “A”, “B”, or “C”). You should use 75% of the dataset to train your classifier, and the remaining 25% for validation (testing). Then, test your trained classifier on each characters in image 1, reporting the final classification results. Do not use the characters in image 2 as training data for your classifier.
Throughout step 8 (training of the classifier), also experiment with pre-processing of the data (e.g., padding/resizing input images) as well as with hyperparameter tuning.
Steps of running the code:

You can just directly run the Proj_1.m and Proj_2.m to see the results, which is very simple.
