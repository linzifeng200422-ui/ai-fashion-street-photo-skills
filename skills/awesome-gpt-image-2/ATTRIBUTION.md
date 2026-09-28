# 来源与署名说明 (Attribution & License)

## 上游项目与版权信息

- **项目名称**：Awesome GPT Image 2
- **上游仓库**：https://github.com/YouMind-OpenLab/awesome-gpt-image-2
- **原作者 / 组织**：YouMind OpenLab
- **开源许可证**：Creative Commons Attribution 4.0 International License (CC BY 4.0)
- **许可证官方全文链接**：https://creativecommons.org/licenses/by/4.0/
- **本地许可证文件**：[references/upstream/LICENSE](references/upstream/LICENSE)

---

## 变更与分发说明 (Indication of Changes)

按照 CC BY 4.0 许可证条款要求，特此说明本技能包对上游原始资源所做的整理变更：

1. **精简为运行所需资源**：
   - 提取了上游仓库的核心多语言提示词索引文档（`README*.md`）、许可证（`LICENSE`）、用户查阅文档（`docs/CONTRIBUTING.md`、`docs/FAQ.md`）以及封面静态图片资源（`public/images/`）；
   - **剔除了开发与构建文件**：排除了 `.git`、`.github`、`.env.example`、`node_modules`、上游 CMS 同步脚本、前端开发构建配置与锁文件（如 `package.json`、`pnpm-lock.yaml`、`tsconfig.json` 等非技能运行时所需内容）。
2. **提示词内容零改动**：
   - 未对上游多语言文档中的任何提示词条目、摄影语法、排版结构或示例进行实质性篡改或重写，保持原汁原味。
3. **定位与边界声明**：
   - 本 Skill 仅作为撰写生图提示词时的**摄影构图、相机视角、布光与质感描述参考库**；
   - 本 Skill **不是生图引擎**，不包含生成能力，也不证明或暗示 Flova、WorkBuddy 等工具底层使用了 GPT Image2 模型。
