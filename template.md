
## 分栏（二栏）

<div class="columns">
  <div class="column">

### 左栏标题
- **核心特性**
  - 代码高亮
  - 数学公式
  - 表格支持

  </div>
  <div class="column">

### 右栏标题

#### 基础设置
- 画布大小：800×480
- 字体：16px
- 内边距：30px

  </div>
</div>


## 任务列表
- [x] 完成基础功能
- [ ] 添加自定义主题
- [ ] 优化长文档渲染


## 复杂表格

| 语法       | 描述                | 示例         |
|------------|---------------------|--------------|
| 标题       | `# H1` 到 `###### H6` | # 标题1      |
| 列表       | `-` 或 `1.`         | - 项目       |
| **强调**   | `**粗体**`          | **重要**     |


## 表格对齐

| 左对齐 | 居中对齐 | 右对齐 |
|:-------|:-------:|-------:|
| 123    | 456     | 789    |


## 数学公式演示

行内公式：$E = mc^2$

块级公式：
$$\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}$$

复杂公式：
$$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$$



积分公式
  $$\int_a^b f(x)dx = F(b) - F(a)$$

求和公式
  $$\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}$$

欧拉公式
  $$e^{i\pi} + 1 = 0$$


## 代码块

```python
import numpy as np
from scipy import integrate

# 数值积分示例
def gaussian(x):
    return np.exp(-x**2)

result, error = integrate.quad(gaussian, -np.inf, np.inf)
print(f"积分结果: {result}")
```

<!-- 使用本地图片 -->
<img src="./2025/11/13/691581ad6c3f0.jpg" width="200" height="150" alt="小图示例">

<!-- Base64 编码的图片 -->
<img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCAEAAQADASIAAhEBAxEB/8QAFQABAQAAAAAAAAAAAAAAAAAAAAv/xAAUEAEAAAAAAAAAAAAAAAAAAAAA/8QAFQEBAQAAAAAAAAAAAAAAAAAAAAX/xAAUEQEAAAAAAAAAAAAAAAAAAAAA/9oADAMBAAIRAxEAPwCdABmX/9k=" width="200" height="150" alt="小图示例">


## 图片尺寸设置示例

### 1. 设置固定宽度和高度
<img src="https://via.placeholder.com/400x200" width="400" height="200" alt="400×200 图片">

### 2. 只设置宽度（高度自动缩放）
<img src="https://via.placeholder.com/600x400" width="300" alt="宽度300px，高度自适应">

### 3. 使用 CSS 样式控制
<img src="https://via.placeholder.com/500x300" style="width: 250px; height: auto; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1)" alt="CSS控制的图片">

### 4. 居中显示图片
<div style="text-align:center; margin: 20px 0">
  <img src="https://via.placeholder.com/300x150" width="300" alt="居中图片">
</div>

## 📌 为什么推荐 HTML `<img>` 标签？

| 方法 | 是否支持 | 优点 | 缺点 |
|------|----------|------|------|
| `<img width="xxx" height="xxx">` | ✅ **完全支持** | 精确控制、兼容性好、在小画布上表现稳定 | 需要写 HTML |
| `![alt](url =200x100)` | ❌ 不支持 | 语法简洁 | Markdown 标准不支持此语法 |
| `![alt](url){width=200}` | ❌ 不支持 | 一些扩展支持 | 本工具不支持此语法 |
| `![alt](url)` | ✅ 支持 | 基础语法 | 无法控制尺寸 |


## 多图并排布局
<div style="display: flex; justify-content: space-between; margin: 20px 0; flex-wrap: wrap">
  <img src="https://via.placeholder.com/150x150" width="150" alt="图1" style="margin-bottom: 15px; border-radius: 6px">
  <img src="https://via.placeholder.com/150x150" width="150" alt="图2" style="margin-bottom: 15px; border-radius: 6px">
  <img src="https://via.placeholder.com/150x150" width="150" alt="图3" style="margin-bottom: 15px; border-radius: 6px">
</div>


## 文字环绕图片
<div style="display: flex; align-items: flex-start; margin: 20px 0">
  <img src="https://via.placeholder.com/120x120" width="120" style="margin-right: 15px; border-radius: 8px" alt="侧边图">
  <div>
    <p>这里是文字内容，图片在左侧，文字环绕显示。这种布局在 800×480 画布上非常实用，能有效利用空间。</p>
    <p>通过设置 width 属性，确保图片在任何设备上都能正确显示。</p>
  </div>
</div>

## 表情符号
😊 🚀 💯 ✅ 🎉

## 关于在 Markdown 中使用 HTML 设置字体

# <span style="font-family:'Microsoft YaHei'; font-size:28px">使用微软雅黑的大标题</span>

普通 Markdown 文本，<span style="font-family:SimSun; color:#e74c3c">这段文字使用宋体和红色</span>。

<div style="text-align:center; font-family:Arial">
  居中对齐的 Arial 字体段落
</div>

| 用途 | HTML 代码示例 | 说明 |
|------|---------------|------|
| 标题字体 | <span style="font-family:'Microsoft YaHei'; font-size:24px">标题</span> | 使用系统常用中文字体 |
| 代码强调 | <span style="font-family:'Courier New'; background:#f0f0f0">代码</span> | 等宽字体+背景色 |
| 警示文本 | <span style="font-family:Arial; color:#e74c3c; font-weight:bold">警告</span> | 红色粗体 |
| 艺术标题 | <span style="font-family:'Brush Script MT'; font-size:36px">艺术字</span> | 手写风格 (注意: 非所有系统都有) |
| 中英混排 | <span style="font-family:'Microsoft YaHei', Arial">中英混合</span> | 设置字体回退 |

## 🌐 常用中文字体 CSS 写法

```css
/* Windows 简体中文 */
font-family: 'Microsoft YaHei', SimSun, SimHei, sans-serif;

/* macOS 简体中文 */
font-family: 'PingFang SC', 'Hiragino Sans GB', 'STHeiti', sans-serif;

/* 通用回退方案 */
font-family: 'Microsoft YaHei', 'PingFang SC', SimSun, Arial, sans-serif;
```


## 三栏布局

<div class="columns">
  <div class="column">

### 第一栏


  </div>
  <div class="column">

### 第二栏


  </div>
  <div class="column">

### 第三栏


  </div>
</div>