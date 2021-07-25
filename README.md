# OpenGL_Learning

## 记录2021年暑假 OpenGL 的学习过程，分享一些学习心得、笔记以及代码

---

### 编译环境
    VS2019 + GLFW + GLEW

### 参考网站
    [link](https://learnopengl-cn.readthedocs.io/zh/latest/)
    
### 环境配置
1. 参考blog : https://blog.csdn.net/Jaihk662/article/details/105496707
- include 文件夹中的内容放入文件夹
	C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.25.28610\include
- lib 文件夹中的内容放入文件夹
	C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.25.28610\lib\x86
- dll 文件夹中的内容放入文件夹
	C:\Windows\SysWOW64、

2. 复制Dependencies文件夹

3. 项目 属性 C++ 链接器 复制路径以及相关文件

4. SOIL  GLM  Assimp

5. shader.vs  shader.frag
    Shader.h  Camera.h  Mesh.h  Model.h
6. 模型、纹理

7. 。。。

### 学习笔记
运行有问题：
1. 检查：  
- 着色器路径
- 资源路径

2. 角度 or 弧度 
- 	使用 glm::radians() 进行转换

3. 初始化矩阵为单位矩阵 
- 	glm::mat4 model = glm::mat4(1.0f);

