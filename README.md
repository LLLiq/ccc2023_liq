ccc2023 为 极光队在ccfSys-ccc2023在提交的CV领域的赛题
其中"filter2D 64x64 image"为基础赛题部分，基于单通道64x64图片filter2D算法的源码。"filter2D HD(1280x720) image"为提高赛题部分，基于单通道720x1080的HD图片filter2D算法的源码

项目构建：
进入对应的源码文件夹使用一下命令可一键编译：
编译最初的的目录默认在项目根目录。
64x64图像项目编译：
```
cd filter2D_64x64_image/aie
make all
cd ../pl
make all
cd ../host
make all
cd ..
make all
```

HD图像项目编译：
```
cd filter2D_HD(1280x720)_image/aie
make all
cd ../pl
make all
cd ../host
make all
cd ..
make all
```

项目运行：
在完成项目构建后，可以使用如下命令快速开始运行：
```
cd host
./template.exe ../build.xilinx_vck5000_gen4x8_qdma_2_202220_1.hw/template.xclbin
```

xclbin:
为了节约编译时间，我们已经将编译好的xclbin文件发送到github的xclbin文件夹
可以进入到对应文件夹使用如下命令快速运行
```
./template.exe ./template.xclbin
```
