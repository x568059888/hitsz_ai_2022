# 哈尔滨工业大学（深圳）2022 年春季学期人工智能 实验
## 实验一 搜索策略pacman
### 实验背景
pacman是加州大学伯克利分校开源的人工智能实验项目，实验
的初衷是在有趣的可视化游戏界面中加入AI策略。
实验地址如下 [CS188 Project1](https://inst.eecs.berkeley.edu/~cs188/su21/project1/)
### 实验目的
通过 pacman 实验，加深对课程介绍的各种搜索算法的理解。
### 实验内容
要求采用但不限于课程第四章内各种搜索算法编写一系列吃豆人程序，解决列出的 8 个搜索问题：
1. 应用深度优先算法找到一个特定位置的豆子
2. 应用宽度优先算法找到一个特定的位置的豆
3. 应用代价一致算法找到一个特定的位置的豆
4. 应用A* 算法找到一个特定的位置的豆
5. 找到所有的角落 —— 基于BFS的角落问题 (CornersProblem Based on BFS)
6. 找到所有的角落 —— 基于A*的角落问题 (CornersProblem Based on A”)
7. 吃掉所有的豆子 —— 食物搜素问题 (FoodSearchProblem）
8. 次最优搜索 —— 任意食物搜素问题 (AnyFoodSearchProblem)
### 实验文件目录层次
.
├── VERSION     
├── autograder.py   
├── commands.txt    
├── eightpuzzle.py  
├── game.py     
├── ghostAgents.py  
├── grading.py  
├── graphicsDisplay.py  
├── graphicsUtils.py    
├── keyboardAgents.py   
├── layout.py   
├── layouts     
├── pacman.py   
├── pacmanAgents.py     
├── projectParams.py    
├── **search.py**   
├── **searchAgents.py**     
├── searchTestClasses.py    
├── submission_autograder.py    
├── testClasses.py  
├── testParser.py   
├── test_cases  
├── textDisplay.py  
└── util.py     
加粗的两个文件是本次实验需要编辑的
### 注意事项
#### `python autograder.py` 报错问题

参考 [AttributeError: module 'cgi' has no attribute 'escape'](https://stackoverflow.com/questions/62470666/getting-this-error-with-py2-7-as-well-as-with-py3-7) 解决。
简单来说，需要在文件中添加语句 `import html`，然后用 `html.escape` 代替
`cgi.escape`

## 实验二 深度学习实现花卉识别

### 实验目的

- 掌握深度学习相关基础知识点，掌握不同神经网络结构，熟悉 其工作原理和实现，如全连接神经网络、卷积神经网络等； 
- 掌握Tensorflow、PyTorch、MindSpore等常用的深度学习框 架，并了解不同框架的区别。

### 实验内容

基于给定的数据集，在本地分别用TensorFlow、MindSpore 、Pytorch框架实现花卉识别

注：必须自己一层层实现模型的定义，不可使用定义好的模型或其他预训练 模型。   

数据集：[](https://gitee.com/hitsz-cslab/AI)

### 实验要求
- 要求必须自己一层层实现模型的定义，不能使用任何定义好的模型 或者其他预训练模型； 
- 可以自行探索预训练模型fine-tune的效果，在实验报告或者答辩中 
- 可以将自定义的模型与其进行对比； 
- 模型在测试集上的精度非唯一评分标准，更注重模型设计、理解、 实现。