# 食物营养查询工具

一个简单的网页应用，可以：
- 文字搜索食物营养信息
- 拍照或上传图片识别食物
- 支持特定食物的精确识别
- 如果不是食物会给出提示
- 移动端友好的界面设计

## 功能特点
- 文字搜索功能
  - 快速查询食物营养成分
  - 支持常见食物快速选择
  - 详细的营养信息展示

- 图片识别功能
  - 支持拍照和上传图片
  - 多模型融合识别
  - 本地图像预处理
  - 用户反馈机制
  - 离线识别支持

## 技术栈
- HTML5
- CSS3
- JavaScript
- Clarifai API (用于图像识别)
- TensorFlow.js (用于本地模型处理)
- IndexedDB (用于本地数据存储)

## 项目结构
```
├── index.html          # 主页面
├── style.css          # 样式文件
├── foodSearch.js      # 食物搜索功能
├── script.js          # 图片识别功能
├── localModel.js      # 本地模型处理
└── database.js        # 数据库操作
```

## 使用说明
1. 文字搜索：
   - 直接输入食物名称
   - 点击常见食物标签
   - 查看详细营养信息

2. 图片识别：
   - 拍照或上传图片
   - 等待识别结果
   - 查看识别详情
   - 提供识别准确度反馈

### API 配置
1. 注册 Clarifai 账号：
   - 访问 https://clarifai.com/signup
   - 完成注册并登录

2. 获取 API 密钥：
   - 进入 Dashboard
   - 点击 "Create Application"
   - 记录下 API Key、App ID 和 User ID

3. 配置项目：
   - 在项目根目录创建 config.js 文件
   - 填入你的 API 配置信息 