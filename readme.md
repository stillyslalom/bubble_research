# Soap fluorescence image processing

## Setting up subfolders
Sets of images should be grouped into top-level folders by shared background conditions.

Each top-level folder must contain three things:

1. A folder containing background images
2. A folder containing signal images
3. A text file "boxes.txt" with the following format:

```
  xrange
  yrange
  xbox
  ybox
```

e.g.

```
  5:142
  1:450
  100:135
  230:270
```

The ranges are the x and y pixel dimensions of the cuvette window
The boxes are the x and y pixel dimensions of the maximum-intensity region within the cuvette window

## Image requirements

All images should be 16-bit greyscale in the .tif fromat, with pixel intensity values in units of counts per second.
