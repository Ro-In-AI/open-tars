# ESP32-S3 固件代码

本目录包含TARS机器人ESP32-S3主控板的固件代码。

## 📁 目录结构

```
2.Firmware/
├── src/                 # 源代码文件
│   ├── main.cpp         # 主程序入口
│   ├── wifi_manager.cpp # WiFi连接管理
│   ├── display.cpp      # OLED显示控制
│   ├── servo_control.cpp# 舵机控制
│   ├── audio.cpp        # 音频处理
│   └── websocket.cpp    # WebSocket通信
├── include/             # 头文件
├── lib/                 # 第三方库
├── platformio.ini       # PlatformIO配置
└── docs/                # 固件文档
```

## 🔧 主要功能模块

- **WiFi管理**: 网络连接和配置
- **显示控制**: OLED屏幕状态和表情显示
- **舵机控制**: SG90舵机动作控制
- **音频处理**: 麦克风输入和音频播放
- **通信协议**: HTTP/WebSocket与后端通信
- **电源管理**: 电池电量监控和省电模式

## 🛠️ 开发环境

- **IDE**: PlatformIO (推荐) 或 Arduino IDE
- **框架**: Arduino Framework
- **芯片**: ESP32-S3
- **编程语言**: C/C++

## 📋 开发状态

- [ ] 基础硬件驱动开发
- [ ] WiFi连接功能
- [ ] 小智AI协议对接
- [ ] OLED显示功能
- [ ] 舵机控制功能
- [ ] 音频录制和播放
- [ ] WebSocket通信
- [ ] 电源管理优化

## 📝 注意事项

请在 `firmware` 分支上进行固件相关的开发工作。

---
*此文件为占位符，具体内容将在开发过程中逐步完善。*