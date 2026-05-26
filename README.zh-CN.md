# 说说输入法 - 专业本地语音输入法

**[English](./README.md)**

一个专业、本地优先的语音输入法，支持 macOS 和 Windows。不绑定供应商，核心能力本地完成，隐私友好。

## 功能特性

- **本地语音识别** - 语音数据不出设备，隐私有保障
- **自定义 AI 服务商** - 支持 10+ 主流 AI 服务商，自由配置
- **自动结构化** - 自动整理文本格式和段落
- **口语过滤** - 智能过滤语气词和重复内容
- **隐私优先** - 零云端数据采集，API Key 仅存本地
- **专业可靠** - 社区驱动，代码可审计

## 技术栈

- **核心语言**: Rust
- **语音识别引擎**: Sherpa ONNX
- **前端框架**: Astro, Tailwind CSS, Alpine.js

## 快速开始

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

## 项目结构

```
/
├── public/           # 静态资源
├── src/
│   ├── components/   # Astro 组件
│   ├── i18n/         # 国际化翻译（中英文）
│   ├── layouts/      # 页面布局
│   ├── pages/        # 路由页面
│   └── styles/       # 全局样式
└── package.json
```

## 相关链接

- 官网：[shuo.us](https://shuo.us)
- GitHub：[shuo-us/shuo-website](https://github.com/shuo-us/shuo-website)

## 开源协议

Apache 2.0
