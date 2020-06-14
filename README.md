# Readme
压缩包内
codes/：
    Yolo：执行Yolo v1
    Faster RCNN：执行Faster RCNN
    SSD ：执行SSD
    test_imgs：测试图片
    
1.下载数据集链接：https://github.com/yukang123/PR_HW_MFD
linux系统使用wget命令 wget https://codeload.github.com/yukang123/PR_HW_MFD/zip/master
Yolo: 1) cd Yolo 2) 使用wget命令下载 3) 解压压缩包 unzip master 4)将解压后的文件夹中的all_data文件夹移动至Yolo项目根目录中5)将移动后的all_data文件夹重命名为data linux系统 mv PR_HW_MFD-master data
Faster RCNN: 1) cd simple-masked-face-faster-r-cnn-pytorch1.0/data 2) 使用wget命令下载 3) 解压压缩包 unzip master 4)将文件夹重命名为AIZOO linux系统 mv PR_HW_MFD-master AIZOO
SSD: 1) 1) cd simple-masked-face-ssd-pytorch/ssd/data/datasets 2) 使用wget命令下载 3) 解压压缩包 unzip master 4)将文件夹重命名为AIZOO linux系统 mv PR_HW_MFD-master AIZOO

2.运行软件环境：
Faster RCNN: python2.7 + pytorch1.0
SSD:python3.6.10 + pytorch1.4

3.使用训练好的模型对测试图片进行测试：
Faster RCNN：1)将test_imgs里的图片全部复制到simple-masked-face-faster-r-cnn-pytorch1.0目录下的demo文件夹
                 或者在demo.py文件中对demo函数输入demo_path = "../test_imgs"
             2) 在simple-masked-face-faster-r-cnn-pytorch1.0目录下运行demo.py
SSD：1)将test_imgs里的图片全部复制到simple-masked-face-ssd-pytorch目录下的demo文件夹
                 或者在demo.py文件中对main函数输入images_dir = "../test_imgs",output_dir ="../test_imgs/results"
             2) 在simple-masked-face-ssd-pytorch目录下运行demo.py

4.训练：
Yolo：在Yolo目录中运行train.py
Faster RCNN: 在simple-masked-face-faster-r-cnn-pytorch1.0目录下运行train_predict.py
SSD: 在simple-masked-face-ssd-pytorch目录下运行train_predict.py

5.在进行完第四步后重复第三步即可使用新训练产生的模型进行测试
