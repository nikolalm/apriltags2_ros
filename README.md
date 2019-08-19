# apriltag2_ros

- 相机驱动

  - usb_cam

    <https://github.com/ros-drivers/usb_cam>

  - 报错select timeout

    解决方案：VMware将USB控制器选项中的 USB 兼容性 选择为 USB 3.0 

- 摄像头标定

  - camera calibration

    <https://github.com/ros-perception/image_pipeline>

  - 流程

    - 参数

      --size 角点数，如图为7x5

      --square 小方块大小，单位m

     ```
      rosrun camera_calibration cameracalibrator.py --size 7x5 --square 0.029 image:=/usb_cam/image_raw camera:=/usb_cam
     ```

       参考博客：<https://blog.csdn.net/weixin_43331257/article/details/82932904>

- apriltags2_ros
  - <https://github.com/shijiwensjw/apriltags2_ros>

  - 参数设置
    
