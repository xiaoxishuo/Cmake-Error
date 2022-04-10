# Cmake-Error
## 1、Unable to find either executable 'empy' or Python module 'em'...  try
- 问题描述：
``` catkin_make```命令报错：CMake Error at /opt/ros/noetic/share/catkin/cmake/empy.cmake:30 (message):   Unable to find either executable 'empy' or Python module 'em'...  try
即使sudo apt install python3-empy也无法解决
- 解决方法：``` catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3 -DPYTHON_INCLUDE_DIR=/usr/include/python3.7m ```

