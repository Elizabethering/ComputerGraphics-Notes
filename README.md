# ComputerGraphics-Notes

![状态](https://img.shields.io/badge/状态-学习中-green)
![语言](https://img.shields.io/badge/语言-C++-00599C?logo=c%2B%2B)
![API](https://img.shields.io/badge/API-OpenGL-5586A4?logo=opengl)
![协议](https://img.shields.io/badge/license-MIT-lightgrey)

## 📖 仓库简介

你好，我是 Elizabethering。本仓库是我学习**计算机图形学 (Computer Graphics)** 的个人空间。

学习图形学需要坚实的理论基础和大量的编码实践。因此，本仓库将整合来自国内顶尖大学的理论课程和国际上广受欢迎的实践教程，旨在构建一个全面而深入的知识体系。

## 💡 学习理念

我的学习方法是“理论指导实践，实践深化理论”。
* 以**中国科学技术大学《计算机图形学》课程**为主线，学习核心理论、渲染管线和数学基础。
* 同步跟随 **learnopengl.com** 和 **B站优秀OpenGL教程**，将理论知识转化为实际的、可运行的 OpenGL 代码，用实践来检验和巩固所学。

## 📚 学习资源

1.  **理论核心 (Theory Core):**
    * **课程:** [2020年中国科学技术大学《计算机图形学》本科课程（刘利刚）](https://www.bilibili.com/video/BV1iT4y1o7oM/)
    * **产出:** 课程核心概念的笔记，存放于 `USTC_CG_Notes` 目录。

2.  **实践主线 (Practical Mainline):**
    * **网站:** [LearnOpenGL](https://learnopengl.com/) (被誉为OpenGL的现代入门圣经)
    * **产出:** 网站每章节的完整代码实现，存放于 `LearnOpenGL_Code` 目录。

3.  **实践补充 (Practical Supplement):**
    * **课程:** [【最好的OpenGL教程之一】](https://www.bilibili.com/video/BV1MJ411u7Bc/)
    * **产出:** 跟随视频敲写的示例代码，存放于 `Bilibili_OpenGL_Code` 目录。

## 🗂️ 仓库结构

```
ComputerGraphics-Notes/
├── USTC_CG_Notes/                  # 中科大《计算机图形学》理论课程笔记
│   ├── 01_Introduction.md
│   ├── 02_Math_Basics.md
│   └── ...
├── LearnOpenGL_Code/               # learnopengl.com 网站的同步代码实现
│   ├── 1_Getting_Started/
│   ├── 2_Lighting/
│   └── ...
├── Bilibili_OpenGL_Code/           # B站OpenGL教程的同步代码实现
│   └── ...
├── Libs/                             # 第三方库 (GLAD, GLFW, GLM, etc.)
├── resources/                        # 资源文件 (纹理, 着色器, 模型等)
│   ├── shaders/
│   └── textures/
├── CMakeLists.txt                    # CMake 构建脚本
└── README.md                         # 本说明文件
```

## 🛠️ 环境配置与编译 (Setup and Build)

本项目使用 C++ 和 OpenGL，并采用 **CMake** 进行跨平台构建。

### 依赖库 (Dependencies)
本项目主要依赖以下第三方库，已将其头文件或源码置于 `Libs/` 目录下：
* **GLFW:** 用于创建窗口和接收输入。
* **GLAD:** 用于加载 OpenGL 函数指针。
* **GLM:** 用于进行向量和矩阵运算的数学库。
* **stb_image:** 用于加载图片作为纹理。

### 编译流程 (Build Process)
1.  克隆本仓库到本地：
    ```bash
    git clone [https://github.com/Elizabethering/ComputerGraphics-Notes.git](https://github.com/Elizabethering/ComputerGraphics-Notes.git)
    ```
2.  安装 CMake 和一个合适的 C++ 编译器 (如 GCC, Clang, MSVC)。
3.  在项目根目录下，创建并进入 `build` 文件夹：
    ```bash
    cd ComputerGraphics-Notes
    mkdir build
    cd build
    ```
4.  运行 CMake 生成构建文件，然后编译：
    ```bash
    # 生成构建文件
    cmake ..

    # 编译 (在 Linux/macOS 上)
    make

    # 或者 (在 Windows 上使用 Visual Studio)
    # 用 Visual Studio 打开生成的 .sln 文件并编译
    ```

## 🙏 致谢

* **刘利刚教授** 及 **中国科学技术大学** 提供的精彩公开课。
* **Joey de Vries** 创建了内容详实、对初学者极其友好的 [learnopengl.com](https://learnopengl.com/)。
* **Bilibili 平台**及相关教程的创作者，让学习资源触手可及。

## 📄 许可 (License)

本仓库采用 [MIT License](LICENSE) 授权。
