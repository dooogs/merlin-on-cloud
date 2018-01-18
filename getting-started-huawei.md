# 创建峰科计算Merlin Compiler实例
从华为云管理控制台创建实例时，选择Merlin Compiler镜像就可以生成带有Merlin 
Compmiler以及Xilinx SDx工具的实例。运行工具时需要使用的license
和环境变量都会自动设置好。记下生成的实例IP。

# 运行Merlin Compiler例子
开一个新的Terminal窗口，运行以下命令，依照make命令的提示来编译和运行vec_add例子
```
$ssh root@<实例IP>
$cd /home/fpga_design/merlin-examples/vec_add/build
$make
**** Merlin Compiler Makefile
**** Copyright (C) 2017 Falcon Computing Solutions, Inc. - All rights reserved.

$ make <target>
Available targets:
           run - Compile and Run TB Executable on CPU (without Acceleration)
       mcc_acc - Use Merlin Compiler to compile the Acceleration Kernel code
    mcc_runsim - Generate kernel binary for simulation on CPU and run it
  mcc_estimate - Get resource and performance estimates
    mcc_bitgen - Generate kernel binary for Acceleration Platform
    mcc_afigen - Generate AFI for AWS F1 FPGA
 mcc_runaccexe - Run TB Executable on Host CPU and Accelerated Kernel on Platform
         clean - Remove all output products (except for bitgen outputs)
```


