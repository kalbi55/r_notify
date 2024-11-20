# r_notify
```markdown
# FiveM 高级通知系统

这是一个为FiveM开发的高级通知系统，提供了美观、可定制的通知界面，支持多种类型和位置的通知显示。

## 主要特性

- 优雅的3D设计效果
- 支持多种通知类型：成功、错误、信息、警告和自定义
- 可自定义通知位置
- 内置进度条设计
- 平滑的动画效果
- 响应式设计，适应不同屏幕尺寸
- 半透明背景，提升层次感
- 毛玻璃效果，增强视觉吸引力

## 安装

1. 将此资源复制到您的FiveM服务器的`resources`文件夹中。
2. 将以下行添加到您的`server.cfg`文件中：
ensure r_notify
```



```plaintext

## 使用方法

在您的Lua脚本中，您可以使用以下方式触发通知：

```lua
exports.r_notify:ShowNotification(title, message, notificationType, duration, position)
```

参数说明：

- `title`: 通知标题
- `message`: 通知内容
- `notificationType`: 通知类型 ('success', 'error', 'info', 'warning', 'custom')
- `duration`: 通知显示时间（毫秒）
- `position`: 通知位置 ('top-right', 'top-center', 'top-left', 'middle-right', 'middle-left', 'center', 'bottom-right', 'bottom-left', 'bottom-center')


示例：
exports.r_notify:ShowNotification("操作成功", "您的更改已保存。", "success", 5000, "top-right")
