1. Set the CROP_SIZE in data.c line 1131. It should be the same as input image size.
2. Replace all files with the original ones in darknet/src, then build darknet.
3. For gaussian blur, add following lines into the config file.
```
[net]
.
.
motionblur=0.5   # probability of motion blur augmentation (float)
motionblurX=15  # kernel size (integer) in x direction (strength of blur)
motionblurY=15  # kernel size (integer) in y direction (strength of blur)
.
.
```