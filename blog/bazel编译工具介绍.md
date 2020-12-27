# Bazel编译工具介绍

bazel特点：构建和测试工具（build & test）

google开源、编译速度更快、支持多种语言编译

高可读的语法

编译快速且可靠：并行&增量编译

支持多个平台

bazel使用：woekspace packages targets

基于workspace，工作区是一个存放了所有源代码和Bazel编译输出文件的目录，也就是整个项目的根目录。工作区下有packages（包括一组源码和一个BUILD文件）

1.在某个目录下创建WORKSPACE空文件，就可以指定为bazel的工作区

2.packages:包含一组源码和一个BUILD文件，一般是项目的子目录

3.repository：含有WORKSPACE的目录为主仓库目录，也可用@表示

4.bazel利用target的概念进行编译，主要编译脚本在BUILD文件中 

5.构建，根据构建规则生成action graph：用于跟踪文件变化，进行增量编译
