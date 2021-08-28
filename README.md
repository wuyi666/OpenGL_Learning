# OpenGL_Learning

## 记录2021年暑假 OpenGL 的学习过程，分享一些学习心得、笔记以及代码

---

### 编译环境
    VS2019 + GLFW + GLEW

### 参考网站
[旧网站（中文）](https://learnopengl-cn.readthedocs.io/zh/latest/)
（该中文网站已有新的网址，但我仍在该旧网站上学习并搭建环境。若参照新的网站搭建的环境，可能无法运行我的代码）
- ==若要运行我的代码，推荐仍然使用旧网站的教程进行环境搭建==

[英文网站](https://learnopengl.com/)
    
### 环境配置
1. 参考blog的前半部分:[OpenGL环境配置（超全整合版）](https://blog.csdn.net/Jaihk662/article/details/105496707)

* include 文件夹中的内容放入文件夹

C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.25.28610\include

- lib 文件夹中的内容放入文件夹

C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.25.28610\lib\x86

- dll 文件夹中的内容放入文件夹

C:\Windows\SysWOW64

---

2. 复制Dependencies文件夹至项目文件夹（.sln文件所在位置）

---

3. 项目属性设置

* 创建一个空项目

* 打开项目属性

* 配置：所有配置  平台：win32

* 项目 属性 C++ 常规 附加包含目录 复制以下路径 $(SolutionDir)Dependencies\GLFW\include;$(SolutionDir)Dependencies\GLEW\include
* 项目 属性 链接器 常规 附加库目录
$(SolutionDir)Dependencies\GLEW\lib\Release\Win32;$(SolutionDir)Dependencies\GLFW\lib-vc2019
* 项目 属性 链接器 输入 复制以下文件
freetype.lib;assimp-vc142-mtd.lib;SOIL.lib;glew32s.lib;glfw3.lib;opengl32.lib;User32.lib;Gdi32.lib;Shell32.lib;

---

4. 
- 新建 src 文件夹
- 添加文件 Application.cpp，并复制粘贴我的 Application.cpp的内容
- 添加文件：Shader.h   Camera.h  Mesh.h  Model.h

5. 扩展配置

* SOIL
* GLM
* Assimp
* freetype

与==1. 参考blog的前半部分==类似，复制对应库中的include文件夹、lib文件夹、dll文件夹至相对应文件夹。


---

6. 新建文件夹shaders,并添加以下文件：
* shader.vs   shader.frag
* skybox.vs  skybox.frag 
* advanced.vs  advanced.frag
    
---



### 学习笔记
运行有问题：
1. 检查：  
- 着色器路径
- 资源路径

2. 角度 or 弧度 
- 使用 glm::radians() 进行转换

3. 初始化矩阵为单位矩阵 
- glm::mat4 model = glm::mat4(1.0f);

