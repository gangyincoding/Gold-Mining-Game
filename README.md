# 🏗️ 黄金矿工 HTML5 游戏

<div align="center">

![黄金矿工](https://img.shields.io/badge/游戏-黄金矿工-FFD700?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-E34C26?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge)
![CSS3](https://img.shields.io/badge/CSS3-Modern-1572B6?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**一个基于 HTML5 Canvas 的经典黄金矿工游戏，采用吉普力动画风格，融合情感化交互设计**

[在线演示](http://localhost:8000) · [查看演示](#-演示) · [快速开始](#-快速开始) · [游戏玩法](#-游戏玩法)

</div>

## 📖 项目简介

黄金矿工 HTML5 游戏是一个完整的网页版经典休闲游戏，采用现代Web技术栈开发。游戏不仅还原了经典的黄金矿工玩法，更融入了创新的情感化设计元素，让传统的游戏体验变得更加生动有趣。

### 🎯 核心特色

- **🎭 情感化矿工角色** - 矿工会根据游戏情况展现不同表情（开心、担心、鼓励）
- **💬 智能气泡提示** - Emoji+文字组合，适时给予玩家反馈和鼓励
- **🎨 吉普力风格UI** - 温暖治愈的视觉设计，圆润可爱的界面元素
- **⚡ 流畅游戏体验** - 60fps动画，精确的物理碰撞检测
- **🎵 动态音效系统** - Web Audio API实时生成的丰富音效

## 🎮 游戏截图

<div align="center">
    <img src="https://typora-picgo-save-image.oss-cn-beijing.aliyuncs.com/typora-imgs/image-20251029231409783.png?text=黄金矿工+游戏界面" alt="游戏界面" width="800">
    <img src="https://typora-picgo-save-image.oss-cn-beijing.aliyuncs.com/typora-imgs/image-20251029231500166.png?text=黄金矿工+游戏界面" alt="游戏说明" width="800">
    <img src="https://typora-picgo-save-image.oss-cn-beijing.aliyuncs.com/typora-imgs/image-20251029231435123.png?text=黄金矿工+游戏界面" alt="游戏界面" width="800">
    <p><em>温暖治愈的吉普力风格游戏界面</em></p>
</div>

## 🚀 快速开始

### 📋 环境要求

- 现代浏览器（Chrome 60+, Firefox 55+, Safari 11+, Edge 79+）
- 本地HTTP服务器（可选，用于本地开发）

### 🛠️ 安装运行

1. **克隆项目**
   ```bash
   git clone https://github.com/gangyincoding/gold-miner-game.git
   cd gold-miner-game
   ```

2. **启动本地服务器**
   ```bash
   # 使用 Python
   python -m http.server 8000

   # 或使用 Node.js
   npx http-server -p 8000

   # 或使用 PHP
   php -S localhost:8000
   ```

3. **开始游戏**

   打开浏览器访问 `http://localhost:8000`，点击"开始游戏"即可开始游玩！

### 🎮 直接游玩

无需安装，直接在支持HTML5的现代浏览器中打开 `index.html` 文件即可开始游戏。

## 🎯 游戏玩法

### 🕹️ 基础操作

| 操作 | 按键/鼠标 | 功能说明 |
|------|-----------|----------|
| 发射钩子 | 🖱️ 鼠标点击 / 空格键 | 在钩子摆动时点击发射钩子 |
| 暂停游戏 | ⏸️ P键 / Esc键 | 暂停或继续游戏 |
| 速度调节 | ⬆️⬇️ 界面按钮 | 实时调整钩子摆动速度 |
| 重新开始 | 🔄 重启按钮 | 重新开始当前关卡 |
| 音效开关 | 🔊🔇 音效按钮 | 开启或关闭游戏音效 |

### 🎯 游戏目标

- **抓取宝物**：控制钩子抓取地下的各种宝物
- **达到目标分数**：在限定时间内获得足够分数
- **关卡进阶**：完成当前关卡目标进入下一关
- **策略规划**：根据物品重量和价值制定最优策略

### 💎 游戏元素

| 物品 | 价值范围 | 重量 | 特殊效果 | 策略建议 |
|------|----------|------|----------|----------|
| 💎 钻石 | 400-600分 | 极轻 | 闪烁效果 | 优先抓取，高回报 |
| 🏆 大金块 | 250-350分 | 很重 | 金属光泽 | 中后期策略性抓取 |
| 🪙 中金块 | 150-200分 | 中等 | 金色反光 | 稳定收益来源 |
| 🪙 小金块 | 50-100分 | 较轻 | 小巧易抓 | 新手友好，快速积累 |
| 🪨 石头 | 10-30分 | 重 | 粗糙纹理 | 避免抓取，浪费时间 |

### 🎭 情感反馈系统

游戏独创的情感化交互系统：

- **连续失败2次**：矿工担心表情 + "哎呀 😅" 气泡提示
- **连续失败3次+**：矿工鼓励表情 + "再试试！💪" 气泡提示
- **时间警告（≤10秒）**：矿工担忧表情 + "时间不多了！⏰"
- **抓到高价值物品（≥200分）**：矿工开心表情 + "太棒了！⭐"
- **关卡完成**：矿工庆祝表情 + "恭喜过关！🎉"

### 🎮 游戏机制

#### 重量系统
不同物品有不同的重量，影响钩子收回速度：
- **轻物品**（钻石）：快速收回，7.0px/帧
- **中等物品**（小金块）：正常速度，4.0px/帧
- **重物品**（大金块）：缓慢收回，1.8px/帧
- **超重物品**（石头）：极慢收回，1.2px/帧

#### 生命值系统
- **3根蜡烛**代表3次生命机会
- **时间耗尽**损失1根蜡烛
- **所有蜡烛熄灭**游戏结束
- **完成关卡**恢复所有蜡烛

#### 关卡设计
- **第1关**：教学关，物品分布合理，难度适中
- **第2关**：增加大金块，提升策略要求
- **第3关**：出现超大金块，考验玩家技巧
- **第4关+**：随机配置，无限挑战模式

## 🛠️ 技术架构

### 📚 技术栈

- **HTML5 Canvas** - 2D图形渲染和动画
- **JavaScript ES6+** - 游戏逻辑和状态管理
- **CSS3** - 现代化UI设计和动画效果
- **Web Audio API** - 实时音效生成和播放

### 🏗️ 系统架构

```
黄金矿工游戏架构
├── 核心游戏引擎
│   ├── 游戏状态管理 (GameState)
│   ├── 物理引擎 (PhysicsEngine)
│   ├── 碰撞检测系统 (CollisionSystem)
│   └── 动画系统 (AnimationEngine)
├── 渲染系统
│   ├── Canvas绘图引擎 (Renderer)
│   ├── 角色绘制系统 (CharacterRenderer)
│   ├── 物品绘制系统 (ItemRenderer)
│   └── UI绘制系统 (UIRenderer)
├── 交互系统
│   ├── 输入管理器 (InputManager)
│   ├── 事件管理器 (EventManager)
│   ├── 音效系统 (SoundSystem)
│   └── 气泡提示系统 (SpeechBubbleSystem)
└── 游戏逻辑
    ├── 关卡管理器 (LevelManager)
    ├── 计分系统 (ScoreSystem)
    ├── 生命值系统 (LifeSystem)
    └── 物品配置系统 (ItemConfig)
```

### 🎨 核心算法

#### 精确的角度计算
```javascript
// 使用 sin/cos 方法确保钩子运动轨迹准确
const angleRad = hook.angle * Math.PI / 180;
const hookTipX = hook.x + Math.sin(angleRad) * hook.length;
const hookTipY = hook.y + Math.cos(angleRad) * hook.length;
```

#### 实时碰撞检测
```javascript
// 矩形边界碰撞检测算法
if (hookTipX >= left && hookTipX <= right &&
    hookTipY >= top && hookTipY <= bottom) {
    // 碰撞发生，执行抓取逻辑
}
```

#### 智能事件触发
```javascript
// 基于时间间隔和冷却时间的事件管理
if (eventType === 'failCatch' &&
    this.failCount >= 2 &&
    now - this.lastBubbleTime > 3000) {
    // 触发失败提示事件
}
```

### 🎵 音效系统

使用 Web Audio API 实时生成的程序化音效：

| 音效类型 | 频率范围 | 持续时间 | 触发场景 |
|----------|----------|----------|----------|
| 钩子下放 | 400-300Hz | 0.5秒 | 发射钩子 |
| 钩子收回 | 300-400Hz | 0.3秒 | 钩子返回 |
| 抓取成功 | 600-800Hz | 0.4秒 | 成功抓取 |
| 得分音效 | 800-1000Hz | 0.6秒 | 获得分数 |
| 关卡完成 | 400-600Hz | 1.0秒 | 过关庆祝 |
| 游戏结束 | 200-100Hz | 1.5秒 | 游戏失败 |

## 🎨 界面设计

### 🌈 吉普力风格设计理念

- **温暖色调**：以金色、棕色为主，营造温馨氛围
- **圆润元素**：所有UI元素采用圆角设计
- **柔和阴影**：适度的阴影增加层次感
- **渐变背景**：温暖的天空渐变色
- **现代毛玻璃**：半透明背景增加质感

### 📱 响应式设计

- **桌面端**：鼠标和键盘双重控制
- **移动端**：触摸屏优化，虚拟按键
- **平板端**：自适应布局，最佳体验

## 📁 项目结构

```
gold-miner-game/
├── 📄 index.html              # 主游戏文件（2600+行）
├── 📄 simple-game.html        # 简化版游戏（参考版本）
├── 📄 README.md               # 项目说明文档
├── 📄 游戏说明.md             # 详细游戏机制
├── 📄 开发规划.md             # 开发记录
├── 📁 .claude/                # 开发配置
│   └── settings.local.json
└── 🐍 server.py              # 本地服务器脚本
```

## 🧪 开发调试

### 🔧 调试功能

游戏内置了丰富的调试功能：

- **控制台日志**：实时输出游戏状态和调试信息
- **性能监控**：帧率和性能数据监控
- **参数调节**：可调整的游戏参数配置
- **错误处理**：完善的错误捕获和提示机制

### 📊 性能优化

- **帧率控制**：稳定60fps渲染
- **内存管理**：自动清理过期对象
- **Canvas优化**：减少重绘，提升性能
- **音频优化**：音频上下文复用，减少延迟

## 📝 更新日志

### v3.0.0 - 情感化交互版本 ✨
**发布日期：2024年10月29日**

#### 🆕 新增功能
- ✨ **情感化矿工角色系统** - 4种不同表情状态
- 💬 **智能气泡提示系统** - Emoji+文字组合反馈
- 🎭 **事件管理系统** - 智能触发游戏事件
- 🎨 **标题动画角色** - 可爱的小矿工和锤子动画

#### 🎨 界面优化
- 🌈 **吉普力风格UI** - 温暖治愈的视觉设计
- 🎪 **现代化界面** - 毛玻璃效果和渐变背景
- 📱 **响应式设计** - 适配各种设备尺寸

#### 🔧 技术改进
- ⚡ **性能优化** - 60fps流畅动画
- 🎵 **音效系统** - Web Audio API实时生成
- 🏗️ **代码重构** - 模块化架构设计

### v2.0.0 - 稳定版本 🚀
**发布日期：2024年10月28日**

#### 🔧 核心修复
- ✅ **角度计算修复** - 解决左右不对称问题
- 🎯 **碰撞检测优化** - 精确的边界检测
- ⚡ **性能提升** - 动画系统优化

### v1.0.0 - 基础版本 🎮
**发布日期：2024年10月27日**

#### 🎮 基础功能
- 🕹️ **核心玩法** - 经典黄金矿工机制
- 💎 **多种物品** - 钻石、金块、石头等
- 🏆 **关卡系统** - 递增难度设计
- 🎵 **基础音效** - 简单的音效反馈

## 🤝 贡献指南

欢迎对本项目做出贡献！请遵循以下步骤：

### 🐛 报告问题
- 使用 [Issues](https://github.com/gangyincoding/gold-miner-game/issues) 报告bug
- 提供详细的复现步骤和环境信息
- 包含截图或错误信息

### 💡 功能建议
- 在Issues中提出新功能建议
- 详细描述功能需求和使用场景
- 讨论技术实现方案

### 🔧 代码贡献
1. Fork 本项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

### 📋 开发规范
- 使用 ES6+ 语法
- 遵循现有的代码风格
- 添加必要的注释
- 确保代码可读性和可维护性

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

- **经典黄金矿工游戏** - 灵感来源
- **吉普力工作室** - 美术风格灵感
- **HTML5 Canvas** - 强大的2D绘图技术
- **Web Audio API** - 实时音频处理能力

## 📞 联系方式

- **项目主页**：[GitHub Repository](https://github.com/gangyincoding/gold-miner-game)
- **在线演示**：[Live Demo](http://localhost:8000)
- **问题反馈**：[Issues](https://github.com/gangyincoding/gold-miner-game/issues)

---

<div align="center">

**🎮 享受游戏，体验温暖治愈的黄金矿工世界！**

Made with ❤️ and JavaScript

</div>