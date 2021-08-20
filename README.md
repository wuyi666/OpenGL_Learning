# OpenGL_Learning

## 记录2021年暑假 OpenGL 的学习过程，分享一些学习心得、笔记以及代码

---
## 编译环境选择 

#### VS2019 + GLFW + GLAD

### 参考网站
[中文网站](https://learnopengl-cn.github.io/)
[英文网站](https://learnopengl.com/)

#### 请直接参考该网站的前两章，一步步配置环境即可

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

