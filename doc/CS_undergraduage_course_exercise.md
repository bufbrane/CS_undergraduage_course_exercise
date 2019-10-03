# 计算机专业本科课程练习

通过参考经典著作，实现下文的任务。

- 目标：串联知识点、学习内部原理、造玩具轮子

- 原则：不追求性能，只追求易懂
- 软件设计目标：简洁且扩展性好的架构



参考书籍：

《计算机体系结构：量化研究方法》

《计算机组成与设计：软硬件接口》

《The RISC-V Instruction Set Manual》

《编译原理》（龙书）

《现代操作系统》

《操作系统设计与实现》

《Linux内核设计与实现》

《Linux内核设计的艺术》

《自己动手写操作系统》

《Inside SQLite》

---



# 1. 设计一套指令集：bbArch

建议从裁剪RISC-V指令集入手



# 2. 设计一个高级语言：bbLang

建议从裁剪C语言入手



# 3. 实现bbArch的VM：bbVM
该VM有自己的vCPU、vMemory、vStorage、vNIC、vSerialPort，支持单步运行，提供调试接口

使用C++编码，宿主平台为x86 Linux



# 4. 实现bbLang的编译器：bbLC

将bbLang编译为二进制指令（交叉编译）

使用C++编码，宿主平台为x86 Linux，使用flex和bison完成编译器前端的构建

后期实现自举



# 5. 用bbLang为bbVM写一个OS：bbOS
建议从仿照Linux内核入手

分时、多用户、多进程、抢占式调度、微内核

仿照POSIX风格的API



# 6. 用bbLang为该OS写一个关系型DB：bbDB
建议从仿照SQLite入手

该DB将集成进OS，作为OS的一部分



