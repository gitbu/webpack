graph TB
根据配置注册插件 --> register[调用compiler.run进入编译阶段]
register --> make[make阶段]
make --> a[调用loader编译代码]
make --> b[搜集依赖关系]
a --> d[关系树]
b --> d
d --> 根据依赖来决定生成的文件有哪些以及每个文件的内容是什么

