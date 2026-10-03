# iKuai plugins

插件源码位于 `plugins/`，由 `build.py` 统一生成 IPK 安装包和插件索引。

插件源地址：<https://baby666666.github.io/plugins/plugins.json>

## 构建

使用 Python 3.11 或更新版本：

```sh
python build.py plugins build
```

安装包生成于 `build/ipk/`，插件索引为 `build/plugins.json`。

## 发布

仓库仅保留 `main` 分支。推送插件源码、构建脚本或发布工作流的变更后，GitHub Actions 自动构建并直接部署到 GitHub Pages，无需 `gh-pages` 分支。也可手动运行发布工作流。

Ttyd 支持 x86_64，管理页面入口为 `plugins/Ttyd/html/index.html`。
