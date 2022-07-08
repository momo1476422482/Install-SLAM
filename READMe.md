This is a guide (not perfect) for the installation of ORB-SLAM (monocular):

-build docker image from docker file 

-build container and enter into /root

-git clone https://github.com/raulmur/ORB_SLAM.git

-install and build diffrent libraries as introduced in https://blog.csdn.net/Fishmemory/article/details/53288140
 boost; opencv; g2o; ros etc
 
 
 ---for the installation of ros : http://wiki.ros.org/indigo/Installation/Ubuntu  as Ubuntu is 14.04
 should modify the .bashrc file as the uploaded one
 
 ---for the installation of opencv :  
  curl -fsSL https://github.com/opencv/opencv/archive/2.4.13.zip -o opencv.zip \
  && unzip opencv.zip \
  && rm opencv.zip \
  && cd $OpenCV_DIR \
  && mkdir release \
  && cd release \
  && cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local .. \
  && make \
  && make install
