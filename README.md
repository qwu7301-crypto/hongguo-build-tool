# 红果搭建工具

基于 Playwright 的红果短剧广告自动化搭建工具，提供 Tkinter GUI 界面，支持安卓/IOS 平台的七留/每留四种搭建配置。

## 功能

- 自动化广告搭建流程（自定义素材 + 监测链接 + 定向包）
- 支持安卓/IOS 双平台
- 支持七留/每留策略切换
- 支持激励视频搭建模式
- 推广链接统计与 Excel 导出
- 实时日志与进度展示

## 环境要求

- Python 3.10+
- Chrome 浏览器（需以调试端口启动）

## 安装

```bash
pip install -r requirements.txt
playwright install chromium
```

## 使用

### 1. 启动 Chrome 调试端口

```bash
chrome.exe --remote-debugging-port=9222
```

### 2. 运行工具

```bash
python 红果搭建工具.py
```

### 3. 数据格式（ids.txt）

```
账户ID1
账户ID2

剧名

点击监测链接
展示监测链接
视频播放监测链接

素材ID1 素材ID2 素材ID3

===

（下一组，用 === 分隔）
```

## 许可证

[MIT License](LICENSE)
