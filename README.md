# VPKOpenCV

Stripped-down dynamic framework build of OpenCV 3.2 whose only purpose is the `contrib/tracking` interface.

**Architectures**  
arm64-iPhoneOS  armv7-iPhoneOS  armv7s-iPhoneOS  x86_64-iPhoneSimulator   
i386-iPhoneSimulator 

**Modules**   
core  imgproc  tracking  video  world  


**Build**  
https://github.com/opencv/opencv/commit/f1c8e04268c046fdf82fb2a9534dd6ee9b5436b1  
with bitcode and infoplist patches from benjonde  
https://gist.github.com/benjohnde/7155910ec3aa3dfec34d12461ab1d822#file-build_opencv_ios-sh  
with tracking interface added from `contrib` with built-in trackers disabled.
 
 
python ./platforms/ios/build_framework.py  --without calib3d --without cudaarithm --without cudabgsegm --without cudacodec --without cudafeatures2d --without cudafilters --without cudaimgproc --without cudalegacy --without cudaobjdetect --without cudaoptflow --without cudastereo --without cudawarping --without cudev --without dnn --without features2d --without flann --without highgui  --without imgcodecs --without java --without js --without ml --without objdetect --without photo  --without python --without shape --without stitching --without superres --without ts  --without videoio --without videostab --without viz     --dynamic