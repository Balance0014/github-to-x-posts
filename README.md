# GitHub → X Posts

一个面向中文 X 内容运营的 Codex Skill：从 GitHub 找适合普通人的工具，核实真实用法与 X 上的同质内容，最后输出有传播力的帖文、媒体顺序和发布前检查项。

它优先寻找视频制作与剪辑等大众场景。判断重点是“读者能用它完成什么”，而非星数或功能数量。方法旨在提高选题与表达质量，不保证曝光或爆款。

## 第一次使用：3 步上手

**1. 准备 Codex。** 需要能联网的 Codex；只要文案时无需登录 X。若想让它把草稿排进 X 编辑器，再提供相应访问方式。没有访问能力时，它应标出未核实的部分。

**2. 安装 Skill。** 在 Codex 新对话中复制这句话，让内置的 Skill Installer 处理仓库根目录：

```text
用 $skill-installer 从 https://github.com/Balance0014/github-to-x-posts 的仓库根目录安装 github-to-x-posts。如果直接下载失败，改用 git 方法。
```

也可以手动安装到 [Codex 文档所列的个人 Skill 目录](https://learn.chatgpt.com/docs/build-skills)：

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/Balance0014/github-to-x-posts.git ~/.agents/skills/github-to-x-posts
```

安装后开启新对话。如果 Codex 没识别到 Skill，重启 Codex 再试。

**3. 复制首条任务：**

```text
用 $github-to-x-posts 找今天适合发中文 X 的 GitHub 工具。优先视频制作和剪辑，目标是普通用户。验证实际可用性、限制和 X 上是否已经有人用相同角度发过。选最值得发的一个，给我可直接复制的帖文，以及媒体顺序、ALT、入口链接和证据。我自己点击发布。
```

它应交付：**一个选题及选择理由、亲测与来源的区别、最终帖文、媒体/ALT 编排、可点击的使用入口和重要限制。** 如果没有合格选题，应说明原因，不编造一个。

## 工作流程

1. 找到有清晰受众、明确成品、适合短视频或前后对比展示的 GitHub 项目。
2. 核实产品入口、使用门槛、收费与限制；可行时亲自完成核心任务。
3. 搜索 X 上已有的中外文内容，寻找仍有新鲜感的普通用户视角。
4. 用有情绪的开场、具体场景、可见结果和可信证据写中文帖文。
5. 交付最终文案、换行与链接顺序、媒体与 ALT；获得授权时可排入 X 编辑器，由账号主人点击发布。

详细指令见 [SKILL.md](SKILL.md)，可复用的检查表见 [选题与成稿工作表](references/run-sheet.md)。

## 事实与素材

亲测、作者演示和推断需要分开标注。复用素材前确认可复用；署名不能代替授权。收费、星数与平台规则等时效信息应在每次使用时重新核实。

本仓库只包含通用方法和空白工作表，不包含账号后台数据、私人实验记录或个人帖子素材。

## License

MIT，见 [LICENSE](LICENSE)。
