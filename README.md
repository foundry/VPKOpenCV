# VPKOpenCV

Stripped-down static framework build of OpenCV 3.4.1 whose only purpose is to run a fully-functioning `contrib/tracking` module. All extraneous dependencies have been stripped out.

**Architectures**  
arm64-iPhoneOS  armv7-iPhoneOS  armv7s-iPhoneOS  x86_64-iPhoneSimulator   
i386-iPhoneSimulator 

**Modules**   
core  imgproc  tracking  
plotvideo  world  


**Build**  
3.4.1 with `tracking` and `plot` modules added from `contrib`
 
It could be built this way:  
python ./platforms/ios/build_framework.py  --without calib3d --without cudaarithm --without cudabgsegm --without cudacodec --without cudafeatures2d --without cudafilters --without cudaimgproc --without cudalegacy --without cudaobjdetect --without cudaoptflow --without cudastereo --without cudawarping --without cudev --without dnn --without features2d --without flann --without highgui  --without imgcodecs --without java --without js --without ml --without objdetect --without photo  --without python --without shape --without stitching --without superres --without ts  --without videoio --without videostab --without viz     --static

But it was _actually_ built by moving all unrequired modules from the `modules` folder.