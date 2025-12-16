# AstrBot Plugins Collection

![GitHub last commit](https://img.shields.io/github/last-commit/vmoranv/AstrBot_Plugins_Collection)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/vmoranv/AstrBot_Plugins_Collection)

## 插件提交

> [!NOTE]
> 请前往三方仓库提交您的插件：[🥳 发布插件](https://github.com/vmoranv-reborn/AstrBot_Plugins_Collection/issues/new?template=PLUGIN_PUBLISH.yml)

## 自动化数据处理脚本

本仓库包含一套自动化脚本，用于定期同步和处理插件数据：

- [check_for_changes](./scripts/transform_plugin_data/check_for_changes/run.sh) - 检查插件数据文件变更情况
- [clean_up](./scripts/transform_plugin_data/clean_up/run.sh) - 清理临时文件
- [commit_and_push_changes](./scripts/transform_plugin_data/commit_and_push_changes/run.sh) - 提交并推送更新到远程仓库
- [configure_git](./scripts/transform_plugin_data/configure_git/run.sh) - 配置 Git 用户信息
- [fetch_original_plugin_data](./scripts/transform_plugin_data/fetch_original_plugin_data/run.sh) - 从原始仓库获取插件数据
- [get_github_api_info_for_repositories](./scripts/transform_plugin_data/get_github_api_info_for_repositories/run.sh) - 获取插件仓库的 GitHub API 信息（星标数、更新时间等）
- [load_existing_cache_for_fallback](./scripts/transform_plugin_data/load_existing_cache_for_fallback/run.sh) - 加载现有缓存作为回退数据
- [pull_latest_changes_before_checking_rebase_with_autostash](./scripts/transform_plugin_data/pull_latest_changes_before_checking_rebase_with_autostash/run.sh) - 拉取最新更改并与本地修改合并
- [summary](./scripts/transform_plugin_data/summary/run.sh) - 生成处理过程总结报告
- [transform_plugin_data](./scripts/transform_plugin_data/transform_plugin_data/run.sh) - 转换插件数据格式并整合仓库信息

这些脚本通过 GitHub Actions 定时运行，确保插件市场数据始终保持最新。