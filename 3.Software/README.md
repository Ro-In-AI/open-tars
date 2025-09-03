# 后端服务代码

本目录包含TARS机器人的后端对话服务代码。

## 📁 目录结构

```
3.Software/
├── flask_backend/       # Flask后端服务
│   ├── app.py          # 主应用入口
│   ├── routes/         # 路由模块
│   ├── models/         # 数据模型
│   ├── services/       # 业务逻辑
│   └── utils/          # 工具函数
├── ai_adapters/        # AI模型适配器
│   ├── openai_adapter.py
│   ├── qwen_adapter.py
│   └── deepseek_adapter.py
├── tts_engines/        # TTS语音合成引擎
│   ├── edge_tts.py
│   └── custom_voice.py
├── websocket/          # WebSocket服务
├── docker/             # Docker配置
├── requirements.txt    # Python依赖
└── config/             # 配置文件
```

## 🔧 主要功能模块

- **Flask Web框架**: RESTful API服务
- **WebSocket服务**: 实时双向通信
- **STT语音识别**: 音频转文字
- **LLM对话引擎**: 多模型支持（OpenAI、Qwen、DeepSeek）
- **TTS语音合成**: 文字转语音（支持自定义语音包）
- **设备管理**: ESP32设备连接和状态管理
- **日志监控**: 系统运行状态监控

## 🛠️ 技术栈

- **后端框架**: Flask + Flask-SocketIO
- **数据库**: SQLite/PostgreSQL
- **消息队列**: Redis
- **容器化**: Docker + Docker Compose
- **AI模型**: OpenAI API、通义千问、DeepSeek
- **语音合成**: Edge-TTS、自训练语音包

## 📋 API接口

### REST API
- `POST /chat/turn` - 对话轮次处理
- `POST /tts` - 文字转语音
- `POST /device/event` - 设备事件上报
- `GET /device/status` - 设备状态查询

### WebSocket
- `/device/ws` - 设备WebSocket连接
- 推送命令: `display`、`motion`、`speak`

## 📋 开发状态

- [ ] Flask基础框架搭建
- [ ] WebSocket通信服务
- [ ] AI模型适配器开发
- [ ] TTS语音合成集成
- [ ] 设备管理功能
- [ ] Docker容器化部署
- [ ] 监控和日志系统
- [ ] API文档编写

## 📝 注意事项

请在 `backend` 分支上进行后端相关的开发工作。

---
*此文件为占位符，具体内容将在开发过程中逐步完善。*