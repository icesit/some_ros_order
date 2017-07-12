# some_ros_order
## Introduction
* help to remember some ros order 
* before using ros, it is highly recommended to follow [tutorial](http://wiki.ros.org/cn/ROS/Tutorials)
0. source .../setup.bash 
   echo $ROS_PACKAGE_PATH #若想用roscd等命令先source
   ros... -h #显示帮助
1. rostopic list #显示现有topic
2. rostopic type [topic] #显示此topic数据类型
3. rosmsg show [data type] #显示2返回读数据类型
4. rosrun rqt_graph rqt_graph #显示当前node的联系
5. rostopic pub -1 [topic] [data type] -- [data] #发布数据3秒
   rostopic pub [topic] [data type] -r 1 -- [data] #以1hz发布数据
6. rosrun rqt_plot rqt_plot #使用图像显示某个topic的曲线
7. rosservice list #显示所有服务
8. rosservice type [service]| rossrv show #显示此服务的输入参数
9. rosservice call [service] [data] #调用某个服务
10. rosparam #与参数服务器相关的操作
11. rosparam dump [filename] #存储参数到文件，dump换load是读取

12. rosrun image_view image_view image:=[topic] #显示图像，或者
    rqt 
