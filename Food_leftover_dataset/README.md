# Food recognition and leftover estimation


## Overview
The benchmark dataset consists of 8 different trays of food, each containing a first course, second course,
side dish, and possibly salad and bread. For each tray, a “before” image is provided with the state of the food immediately after placing the order, and several “after” images with the presence of leftovers in the tray.
In the `food_categories.txt` file you can find the detailed list of food items in each tray.

The benchmark dataset contains 3 “after” images for each tray, categorized by level of difficulty:

1. Dishes and objects in the same position on the tray for the “before” and “after” images;
2. Dishes and objects in a different order on the tray between the "before" and "after" images, but food
only partially eaten (i.e., looking very similar between the "before" and "after" images);
3. Dishes and objects in a different order on the tray between the "before" and "after" pictures, and
minimal leftover food

## Food categories

The benchmark dataset includes a total of 14 food categories. Each category is assigned to a unique food ID:

0. Background

1. pasta with pesto
2. pasta with tomato sauce
3. pasta with meat sauce
4. pasta with clams and mussels
5. pilaw rice with peppers and peas

6. grilled pork cutlet
7. fish cutlet
8. rabbit
9. seafood salad

10. beans
11. basil potatoes
12. salad
13. bread


## Dataset structure

The dataset is organized as the following. A folder is provided for each tray, containing:

- an image of the tray before the meal (`food_image.jpg`);
- an image of the tray with large food leftover, with dishes in the same position (`leftover1.jpg`);
- an image of the tray with large food leftover, with dishes in different position (`leftover2.jpg`);
- an image of the tray with minimal food leftover, with dishes in the different position (`leftover3.jpg`);
- a `bounding_boxes` folder containing the bounding box annotations of each image;
- a `masks` folder containing the segmentatio mask annotations of each image.


