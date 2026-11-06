# 知识工作流：让笔记找到使用场景

本技能将既有学习材料重写为独立方法笔记，不是原文复刻。说明、步骤与边界均可在本仓库内阅读：[方法笔记](references/methods.md)。

## 什么时候用

笔记存得多却找不到使用入口，或想从零搭一套轻量本地知识库。

## 需要给什么

指定目录或现有目录说明、一个要完成的任务、至少一份样例材料。只有建议需求时不需要文件路径。

## 怎么调用

```text
$lany-knowledge-workflow-skill
这是虚构方案练习：我已有“项目”“摘录”“自己的笔记”三个目录，想让摘录能用于下周的分享。只给方案，不要建目录，不要迁移。
```

## 示例结果（虚构演示）

保留三个目录。项目里记录“给新人解释报销流程”的目标和受众；摘录保留来源；自己的笔记中增加一张说明流程卡。
样例链：从摘录找报销规则→核对当前适用范围→用自己的话写三个步骤→链接回原文→放进分享草稿→记录听众未理解之处。
新增的不是整套分类，而是一条索引记录：用途、当前状态、卡片路径与来源。
验收：新人能沿卡片找到材料并完成演练；如果规则本身过期，先核对规则而非美化卡片。
本例仅为方案，未写入或验证任何真实目录。


## 交付与边界

技能会提供具体判断、动作和验证方式。它不会把示例当成你的经历，也不会仅凭作者的成功故事承诺结果。文件创建或更新仅在当前任务确有需要且范围明确时进行。

[查看完整技能定义](SKILL.md)。

## 补充用法

增加先检索旧卡与未解问题、内容/格式双层验收、单节点失败回填，减少重复囤积。

调用示例：`$lany-knowledge-workflow-skill 这批笔记先检查哪些能补已有问题，只处理与本周分享有关的材料，保留原始资料。`

[阅读方法笔记](references/methods.md)。

## 独立仓库与安装

仓库：[lany-knowledge-workflow-skill](https://github.com/LanyXiaosheng/lany-knowledge-workflow-skill)。本仓库根目录即技能目录，包含 `SKILL.md`、本说明及 `references/`。

确认目标目录不存在后，可在未设置 `CODEX_HOME` 的默认环境下安装：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/LanyXiaosheng/lany-knowledge-workflow-skill.git ~/.codex/skills/lany-knowledge-workflow-skill
```

已设置 `CODEX_HOME` 时，将目标改为该目录下的 `skills/lany-knowledge-workflow-skill`。已有同名技能时先比较或备份，不覆盖。客户端发现技能后，使用 `$lany-knowledge-workflow-skill` 调用。

当前版本附自包含方法笔记，无需访问外部原文；现有仓库提交历史保留。

## 操作手册

[本地操作手册](references/workbook.md)包含可填写模板、完整虚构案例、反例与验收步骤，可与方法笔记配合使用，无需访问原文网站。
