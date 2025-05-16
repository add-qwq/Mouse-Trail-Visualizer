# English:
# Mouse Trail Visualizer  

## Introduction  
A lightweight HTML5 Canvas project that visualizes mouse movement trajectories in real time. When users move the mouse on the page, it generates dynamic, colorful trails with fading effects, creating an intuitive and visually appealing cursor interaction feedback. The trails automatically fade out over time, and the canvas adapts to window size changes.  

## Features  
- **Real-Time Tracking**: Continuously captures mouse movement coordinates and draws trails in real time.  
- **Dynamic Colors**: Uses sine wave algorithms to generate RGB colors, creating constantly changing rainbow-like trails.  
- **Auto-Resizing**: The canvas automatically adjusts to match window dimensions, ensuring full-screen coverage.  
- **Fade-out Animation**: Trails gradually fade and disappear after approximately 2 seconds (configurable via `age` threshold in code).  
- **Visual Effects**: Includes shadow blur and round-end line caps for smooth, soft trail edges.  

## Usage  
1. **Download**: Save the provided `鼠标轨迹.html` file to your local directory.  
2. **Open in Browser**: Double-click the file or open it in a modern browser (Chrome/Firefox/Edge, etc.).  
3. **Interact**: Move the mouse on the page to see dynamic trails; resize the window to test auto-resizing.  

## Customization  
Adjust parameters in the JavaScript code to modify the effect:  
- `trailPoints.length`: Control the maximum number of trail points stored (affects trail density).  
- `age > 400`: Modify the trail survival time threshold (in milliseconds, default: 400ms).  
- `alpha = 1 - (age / 2000)`: Adjust the fade-out speed by changing the denominator (e.g., increase to 3000 for slower fading).  
- `lineWidth`/`shadowBlur`: Tweak values in `drawTrail()` to change trail thickness and shadow intensity.  

## Technical Details  
- **Canvas API**: Uses HTML5 Canvas 2D context for rendering.  
- **Performance**: Optimized with `requestAnimationFrame` for smooth animations.  
- **Event Handling**: Listens for `mousemove` and `resize` events for real-time updates.  

# 中文：
# 鼠标轨迹可视化工具  

## 项目简介  
一个轻量级HTML5 Canvas项目，用于实时可视化鼠标移动轨迹。当用户在页面移动鼠标时，会生成动态彩色轨迹并伴随淡化效果，提供直观的光标交互视觉反馈。轨迹随时间自动淡出，画布支持窗口尺寸自适应。  

## 功能特性  
- **实时跟踪**：持续捕获鼠标移动坐标并实时绘制轨迹。  
- **动态色彩**：通过正弦波算法生成RGB颜色，形成不断变化的彩虹般轨迹。  
- **自动适配**：画布自动调整尺寸以匹配窗口，支持全屏显示。  
- **淡出动画**：轨迹约2秒后逐渐淡化消失（可通过代码中`age`阈值配置）。  
- **视觉效果**：包含阴影模糊和圆形线帽，使轨迹边缘平滑柔和。  

## 使用方法  
1. **下载**：将提供的`鼠标轨迹.html`文件保存至本地目录。  
2. **浏览器打开**：双击文件或在现代浏览器（Chrome/火狐/Edge等）中打开。  
3. **交互体验**：在页面移动鼠标查看动态轨迹；调整窗口大小测试自适应功能。  

## 自定义配置  
通过修改JavaScript代码中的参数调整效果：  
- `trailPoints.length`：控制存储的轨迹点数上限（影响轨迹密度）。  
- `age > 400`：修改轨迹存活时间阈值（单位毫秒，默认400ms）。  
- `alpha = 1 - (age / 2000)`：通过调整分母改变淡出速度（如改为3000可减缓淡化）。  
- `lineWidth`/`shadowBlur`：在`drawTrail()`中修改数值调整轨迹粗细和阴影强度。  

## 技术细节  
- **Canvas API**：基于HTML5 Canvas 2D上下文实现渲染。  
- **性能优化**：使用`requestAnimationFrame`实现流畅动画。  
- **事件监听**：通过监听`mousemove`和`resize`事件实现实时更新。  
