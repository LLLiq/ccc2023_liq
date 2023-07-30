ccc2023 为 极光队在ccfSys-ccc2023在提交的CV领域的赛题
其中"filter2D_8K"为源代码部分

项目构建：
进入对应的源码文件夹使用以下命令编译：
编译最初的的目录默认在项目根目录。
```
cd filter2D_8K/aie
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

quick_start:
为了节约编译时间，我们已经将编译好的xclbin文件发送到github的xclbin文件夹
可以进入到对应文件夹使用如下命令快速运行
```
./template.exe ./template.xclbin
```
