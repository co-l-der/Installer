#### 一个简单的安装包制作教程

- reference: https://www.cnblogs.com/gongdiwudu/p/11070798.html
- reference: http://blog.konghy.cn/2018/04/29/setup-dot-py/

1. 在项目下新建一个setup.py

2. 执行python setup.py sdist bdist_wheel
   说明：执行成功后，会在当前目录下生成三个文件夹,如下
   1). build
   2). dist: 存放tar.gz和whl安装包
   3). demo.egg-info
   
3. 进入dist, 安装制作的安装包
   pip install demo-0.0.1-py3-none-any.whl
   
4. 验证安装包， 如果没报错，则安装包制作成功
   from demo import run
   run.say_hello("wang")
   
5. 写调用示例， 参考步骤4

6. 写readme文档
