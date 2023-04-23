# ME5405
**NUS ME5405 Module - Machine Vision**

Images 1 and 2 are 64x64, 32 level images. These images are shown as coded arrays that contains an alphanumeric character for each pixel. The range of these characters is 0-9 and A-V, which corresponds to 32 levels of gray.

Image 1:

For Image1 ```(chromo.txt)```, the main function file is ```Project_1.m```.

Perform the following tasks:

1. Display the original image on screen.
```javascript
function [histogram_num, small_gray_img, gray_img] = original_image(filepath)
```

2. Threshold the image and convert it into binary image.
```javascript
function [small_gray_img, gray_img] = binary_image(histogram_num)
```

3. Determine an one-pixel thin image of the objects.
```javascript
function [no_pad, no_pad_enlarged] = onepixel_image(binary)
```
4. Determine the outline(s).

First method
```javascript
function [outline_img, outline_enlarged] = outline_image(binary)
```
Second method
```javascript
function [height, width,output] = canny_edge_detection(input_image)
```
Label the different objects. Discuss and compare 4-connectivity and 8-connectivity in your report.




Image 2: 

For Image1 ```(charact.txt)```, the main function file is ```Project_2.m```.

Perform the following tasks:

1. Display the original image on screen.
```javascript
function [histogram_num, small_gray_img, gray_img] = original_image(filepath)
```

2. Create a binary image using thresholding.
```javascript
function [small_gray_img, gray_img] = binary_image(histogram_num)
```

3. Determine a one-pixel thin image of the characters.
```javascript
function [no_pad, no_pad_enlarged] = onepixel_image(binary)
```

4. Determine the outline(s) of characters of the image.

First method
```javascript
function [outline_img, outline_enlarged] = outline_image(binary)
```
Second method
```javascript
function [height, width,output] = canny_edge_detection(input_image)
```
Label the different objects. Discuss and compare 4-connectivity and 8-connectivity in your report.

Segment the image to separate and label the different characters.

Arrange the characters in one line with the sequence: AB123C

Rotate the output image from Step 6 about its center by 30 degrees.

Using the training dataset (p_dataset_26.zip), train the (conventional) unsupervised classification method of your choice (Here k-nearest neighbors (kNN) is used) to recognize the 6 characters (“1”, “2”, “3”, “A”, “B”, or “C”). You should use 75% of the dataset to train your classifier, and the remaining 25% for validation (testing). Then, test your trained classifier on each characters in image 1, reporting the final classification results. Do not use the characters in image 2 as training data for your classifier.

Throughout step 8 (training of the classifier), also experiment with pre-processing of the data (e.g., padding/resizing input images) as well as with hyperparameter tuning.



You can just directly run the project_1.m and project_2.m to see the results, which is very simple.
