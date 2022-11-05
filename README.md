# SingleFileExecutionPlugin

## 用途

可以将单个 cpp 文件加入到 CMakeLists.txt 中


## feature

我这个使用的是 uuid 作为 target

另外文件名可能包含中文和空格, 所以文件和目标都用引号括起来了


## IDEA 插件

需要安装高点版本的 JDK, 然后使用 IDEA plugin SDK

2022 建议使用  JDK 11

## 构建

`构建 -> 重新构建项目` 可以在项目目录下的out目录得到编译的结果，需要自己打包成  jar 包：

在目录： `PS D:\IdeaProjects\SingleFileExecutionPlugin\out\production\SingleFileExecutionPlugin\META-INF` 下执行：

```bash
jar cvfm SingleFileExecutionPlugin.jar  .\MANIFEST.MF  -C  \
        D:\IdeaProjects\SingleFileExecutionPlugin\out\production\SingleFileExecutionPlugin/ .

```


