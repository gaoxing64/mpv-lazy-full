# MPV-Lazy

MPV-Lazy是一个功能丰富的MPV播放器预配置包，旨在为用户提供开箱即用的高级视频播放体验。通过集成多种实用脚本和优化设置，MPV-Lazy提供了丰富的功能，如高质量视频渲染、进度条缩略图预览、视频补帧和超分辨率等。

## 与原版mpv-lazy的主要区别

### 1. 界面优化
- 采用uosc替代原版的osc，提供更现代化的界面体验
- 优化了进度条显示和缩略图预览的视觉效果
- 改进了控制面板的布局和交互方式

### 2. 补帧算法升级
- 新增RIFE_RTX补帧支持，提供更高质量的补帧效果
- 优化了MVTools补帧参数，提升补帧质量
- 新增SVP补帧支持，提供更多补帧选择

### 3. 超分辨率增强
- 新增ESRGAN_DX12和ESRGAN_RTX超分支持
- 优化了超分算法的性能表现
- 提供更多超分预设选项

### 4. 着色器系统改进
- 重新组织了着色器结构，分为LUMA、CHROMA和OUTPUT三类
- 新增自适应锐化着色器
- 优化了着色器的加载和切换机制

### 5. 快捷键系统优化
- 重新设计了快捷键布局，更符合使用习惯
- 新增更多实用快捷键，如缩略图控制
- 优化了快捷键的响应速度

### 6. 性能优化
- 优化了硬件解码配置
- 改进了内存管理机制
- 提升了整体播放性能

## 主要特性

- **现代化界面**：整合uosc脚本，提供简洁美观的用户界面
- **进度条缩略图预览**：使用thumbfast引擎，在进度条上提供实时缩略图预览
- **高级视频处理**：
  - 补帧：支持多种补帧算法（MVTools、RIFE、SVP）
  - 超分辨率：支持ESRGAN、WAIFU等超分辨率算法
  - 降噪：内置多种降噪算法
- **丰富的着色器**：包含多种LUMA、CHROMA和OUTPUT着色器，可提升视频画质
- **全面的键盘快捷键**：详尽的快捷键设置，方便操作和控制
- **播放速度控制**：灵活的播放速度调整，支持预设和精细调节
- **视频均衡器**：内置视频参数调整，包括对比度、亮度、饱和度等

## 快速开始

1. 下载最新版本的MPV-Lazy
2. 解压到任意位置
3. 运行mpv.exe开始使用

## 常用快捷键

查看项目中的`mpv快捷键表.md`或`mpv快捷键表.html`获取完整快捷键列表。一些常用快捷键：

- **SPACE**: 播放/暂停
- **LEFT/RIGHT**: 快退/快进5秒
- **UP/DOWN**: 前进/后退1秒
- **{/}**: 调整播放速度(1-8x)
- **[/]**: 精细调整播放速度(±0.1)
- **BS**: 重置播放速度
- **Ctrl+o**: 开启/关闭缩略图预览
- **F1-F6**: 控制OUTPUT着色器
- **Ctrl+`**: 清除所有着色器
- **~**: 清除所有滤镜

## 高级功能

### 视频补帧

MPV-Lazy集成了多种视频补帧算法，可以通过快捷键快速启用：

- **!**: MVTools快速补帧
- **@**: MVTools标准补帧
- **SHARP**: RIFE标准补帧
- **$**: RIFE_RTX补帧
- **Alt+1/2**: SVP补帧

### 超分辨率

支持多种超分辨率算法，提升视频分辨率和清晰度：

- **%**: ESRGAN_DX12超分
- **^**: ESRGAN_RTX超分
- **Alt+3/4/5**: 更多超分选项

### 着色器

丰富的着色器预设，可根据需要启用不同效果：

- **Ctrl+1-4**: LUMA着色器
- **Ctrl+5**: CHROMA着色器
- **Ctrl+6-8**: 主要着色器
- **Ctrl+9/F1-F6**: OUTPUT着色器

## 自定义配置

主要配置文件位于portable_config目录：

- **mpv.conf**: 主配置文件
- **input.conf**: 键盘快捷键配置
- **input_uosc.conf**: uosc界面快捷键配置
- **script-opts.conf**: 脚本选项配置

## 缩略图预览配置

缩略图预览功能通过thumbfast脚本提供，配置位于：

- **portable_config/script-opts/thumbfast.conf**

主要参数包括：缩略图尺寸、硬解设置、生成精度等。

## 系统要求

- Windows 7/10/11
- 推荐4GB以上内存
- 独立显卡（使用硬件解码和高级处理功能时）

## 鸣谢

感谢以下项目和贡献者：

- [MPV播放器](https://mpv.io/)
- [uosc脚本](https://github.com/tomasklaen/uosc)
- [thumbfast脚本](https://github.com/po5/thumbfast)
- [原版mpv-lazy项目](https://github.com/hooke007/MPV_lazy)
- 所有为MPV社区贡献的开发者 
=======
# mpv-lazy-full
