# NOVAIR FluxDock — AI 视觉设计案例

这是一个用于应聘 3C 产品 AI 设计岗位的个人概念设计练习，不是任何真实品牌或官方项目。

Self-initiated concept project. Not affiliated with any commercial brand.

NOVAIR FluxDock 是虚构品牌和概念产品。本项目用于展示 AI 辅助视觉设计、产品画面、场景设计和广告分镜能力；不代表真实上市产品，不使用虚构销量、参数、专利或用户评价。

## 项目定位

为海外年轻消费者、手游用户和移动办公人群设计一款虚构的磁吸手机散热器：NOVAIR FluxDock。
核心信息不是承诺无法验证的性能数字，而是「贴合、轻薄、安静、专注」的使用体验。

- 目标用户：手游玩家、通勤中的内容消费者、移动办公人群
- 核心场景：游戏、通勤、桌面办公
- 视觉主方向：极简国际化（Light / Space / Focus）
- 辅助探索：科技冷感、运动电竞
- 语言：网页与商业视觉采用英文主版本；过程文档保留中文说明，便于复盘

## 工具与工作方式

- AI 图像生成：OpenAI 内置 image generation（先建立产品母版，再以母版为一致性参考生成场景）
- 二次设计：HTML/CSS 排版、SVG 产品示意、裁切、颜色统一、文案人工排版
- 检查：PowerShell 文件检查、浏览器可运行的静态网页结构检查
- 未使用真实品牌 Logo、商标、宣传语、销量、用户评价、奖项、专利或未验证技术参数

## 工作过程

1. 需求分析：拆解目标人群、场景、痛点与卖点。
2. 风格探索：科技冷感 / 运动电竞 / 极简国际化三方向并列比较。
3. 产品母版：确定 FluxDock 的圆角矩形轮廓、银白金属边、深石墨背板、居中磁吸环、单侧按键与底部 USB-C 口。
4. AI 生成：先生成母版与产品场景，再针对渠道比例生成构图。
5. 方案筛选：选择极简国际化作为主方向，保留另两套探索记录。
6. 二次设计：所有商业文案放入网页排版层，统一边距、字号、对比度和信息层级。
7. 多尺寸适配：16:9、1:1、4:5、9:16，以及详情页模块化适配。
8. 方法沉淀：在 `PROMPT_LOG.md` 中记录提示词、迭代、淘汰理由和一致性检查清单。

## 文件结构

```text
novair-fluxdock-case/
├─ README.md
├─ PROMPT_LOG.md
├─ index.html
├─ styles.css
├─ assets/
│  ├─ generated/       # AI 生成的视觉素材
│  ├─ master/          # 产品母版、透明产品图、提示词
│  └─ exports/         # 可交付尺寸说明与导出说明
└─ docs/
   ├─ visual-strategy.md
   └─ storyboard.md
├─ FINAL_QA.md
├─ VIDEO_EDIT_GUIDE.md
├─ exports/
│  └─ final/            # 独立 PNG 导出：hero / ecommerce / social / scenes / product-master / before-after / detail-page / video
└─ tools/
   └─ export-final.ps1  # 可复现的最终导出脚本
```

## 人工确认项

- 真实求职时需要根据岗位 JD 调整自我反思与个人贡献叙述。
- 若进入生产阶段，需要用真实工程样机确认磁吸强度、散热路径、噪音、兼容机型与安全认证。
- AI 生成场景仍需在最终投递前逐张检查手指、接口、边缘、反射和屏幕内容。
- 本项目的英文文案为概念文案，不代表真实产品规格或性能结论。

## 最终验收与导出

- `FINAL_QA.md`：逐张验收、问题位置、处理方式与结果。
- `VIDEO_EDIT_GUIDE.md`：15 秒剪映时间轴、转场、字幕、音效和导出设置。
- `CAPCUT_EDIT_GUIDE.md`：中文剪映制作步骤和视频素材说明。
- `exports/final/`：独立 PNG 成品，已按用途分目录并写入 `export-manifest.json`。
- `exports/final/video-edit-package/`：7 张分镜图、无文字场景图、字幕文件和剪映指南。
- `exports/final/video/`：15 秒有声版、静音版、封面 JPG 和验收截图。
- `tools/build-video.ps1`：使用 D 盘便携版 FFmpeg 生成两版 MP4 的可复现脚本。
- `output/pdf/LU-Jinying_NOVAIR-FluxDock_AI-Visual-Case.pdf`：12 页横版投递版作品集 PDF。
- `publish/`：适用于 GitHub Pages 或 Cloudflare Pages 的静态发布目录，仅包含网页运行所需资源。
- 原始 AI 素材没有被删除，仍保留在 `assets/generated/`，用于展示生成过程和二次设计边界。
