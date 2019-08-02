# get_moves

## 使用说明

- 安装依赖项 `conda install pybind11` （注意`pip install`不行，因为不会安装下面`cmake`操作中所需要的`.cmake`文件，如果你没装anaconda，就去官网自己下载pybind11，然后`build, cmake, make install`）

- 运行
    ```bash
    mkdir build
    cd build
    cmake ..
    ```

- 会根据自己系统环境在`build`创建相应项目，然后

    - Windows下的话，用vs打开`r.sln`，然后build一个`x64`的`Release`方案即可

    - \*Unix 没试过

- 然后，Windows下在`build/Release`目录下会有一个`r.xxx.pyd`文件，把这个文件复制出去，使它和你代码目录一致，代码直接`import r`即可使用。效果如下：

    ![效果图](https://github.com/deecamp2019-group20/bottleneck/blob/master/get_moves/%E6%95%88%E6%9E%9C.png)

- 如果`precompile`文件夹下没有你适合的，你编译生成后，放里面传上来

- 其他不懂的，来353-3找我
