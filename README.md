# some_ros_order
## Introduction
* help to remember some ros order 
* before using ros, it is highly recommended to follow [tutorial](http://wiki.ros.org/cn/ROS/Tutorials)
0. 基本指令
 > source .../setup.bash 
 > echo $ROS_PACKAGE_PATH 
 > ros... -h 
1. 显示现有topic 
 > rostopic list 
2. 显示此topic数据类型
 > rostopic type [topic]
3. 显示2返回读数据类型
 > rosmsg show [data type]
4. 显示当前node的联系
 > rosrun rqt_graph rqt_graph
5. 发布数据3秒
 > rostopic pub -1 [topic] [data type] -- [data]
   以1hz发布数据
 >  rostopic pub [topic] [data type] -r 1 -- [data] 
6. 使用图像显示某个topic的曲线
 > rosrun rqt_plot rqt_plot
7. 显示所有服务
 > rosservice list
8. 显示此服务的输入参数
 > rosservice type [service]| rossrv show
9. 调用某个服务
 > rosservice call [service] [data]
10. 与参数服务器相关的操作
 > rosparam
11. 存储参数到文件，dump换load是读取
 > rosparam dump [filename]
12. 显示图像
 > rosrun image_view image_view image:=[topic]
    
    或者
 >  rqt 
