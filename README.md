# PatentMarker — Word → PowerPoint / Visio

PatentMarker 包含 Word → AutoCAD、Word → PowerPoint、Word → Visio 三条标注路线。**源码、公共代码、构建与使用说明统一维护于 [PatentCAD-Annotator 主仓库](https://github.com/Wujiamu/PatentCAD-Annotator)。** PPT / Visio 位于其中的 `office-com-addin/`，两端分别打包安装。

| 使用端 | 打开标注面板 | 使用说明 |
|---|---|---|
| PowerPoint | 安装后完全退出并正常重新启动，自动显示“专利标注字典工具 · PowerPoint” | [PPT 说明](https://github.com/Wujiamu/PatentCAD-Annotator/blob/master/office-com-addin/ppt-release-readme.md) |
| Visio | 安装后完全退出并正常重新启动，自动显示“专利标注字典工具 · Visio” | [Visio 说明](https://github.com/Wujiamu/PatentCAD-Annotator/blob/master/office-com-addin/visio-release-readme.md) |

面板关闭或最小化后，从 Windows 任务栏或 `Alt+Tab` 恢复。未出现面板时，按[面板入口与故障排查](https://github.com/Wujiamu/PatentCAD-Annotator/blob/master/office-com-addin/docs/open-annotation-panel.md)检查 COM 加载项。

三条路线共用 Word 导出的 `.dict.json` 和同一份编号比较源码；PPT / Visio 另共用字典读取、日志与 COM 接口。各宿主的标注和文档绑定实现分别维护，详见[项目架构](https://github.com/Wujiamu/PatentCAD-Annotator/blob/master/docs/project-family.md)。