# NOVAIR FluxDock / 剪映制作指南

这是一个可直接整理进剪映的 15 秒竖屏素材包。素材只表达产品关系、使用场景和专注感，不包含未经验证的降温数值、噪声数值、销量、认证或效果承诺。

## 项目设置

- 画布：1080 x 1920，9:16
- 帧率：30 fps
- 总时长：15.0 秒
- 素材目录：`exports/final/video-edit-package/`
- 分镜目录：`storyboards/`
- 无文字场景图：`scene-assets/`
- 单独字幕：`captions.txt` 和 `captions.srt`

## 时间轴

| 镜头 | 时间 | 文件 | 字幕 | 动作与转场 |
|---|---|---|---|---|
| 01 | 0.0-1.8s | `01-hook.png` | A cooler way to stay in the moment. | 从 92% 推至 100%，前 0.5 秒保持稳定；0.12 秒淡入。 |
| 02 | 1.8-4.0s | `02-magnetic-fit.png` | Magnetic fit. | 对磁吸圆环 104% 推至 100%；与上一镜头做中心 match cut。 |
| 03 | 4.0-6.2s | `03-gaming.png` | Built for long sessions. | 轻微左右 2 度摇镜；4 帧硬切，避免快速抖动。 |
| 04 | 6.2-8.4s | `04-commute.png` | Pocket-ready form. | 横向平移约 18px；横向擦拭转场。 |
| 05 | 8.4-10.8s | `05-desk.png` | Quiet focus. | 轻微下移约 14px；0.2 秒交叉溶解。 |
| 06 | 10.8-13.0s | `06-hero.png` | One clean setup. | 100% 推至 106%，最后 0.4 秒固定产品中心；银色边框 match cut。 |
| 07 | 13.0-15.0s | `07-endcard.png` / `scene-assets/endcard-base.png` | NOVAIR FluxDock<br />Magnetic Mobile Cooling Concept<br />Self-initiated concept project. | 深色品牌结束画面；三行英文文案 0.3 秒淡入；0.25 秒淡出。 |

总时长计算：1.8 + 2.2 + 2.2 + 2.2 + 2.4 + 2.2 + 2.0 = 15.0 秒。

## 剪映操作步骤

1. 新建 1080 x 1920、30 fps 项目。
2. 将 `storyboards/` 中 7 张图片按 01-07 顺序放入主轨。
3. 手动设置每张图片时长，确保时间轴显示 15.0 秒。
4. 按上表添加关键帧：只做轻微推近、平移和缩放，不使用夸张 3D 转场。
5. 分镜图已经包含字幕。若在剪映中重新排字幕，只保留一套字幕，不要叠加重复字幕。
6. `scene-assets/` 中的无文字场景图可用于重新剪辑或替换画面；替换时保持产品比例与构图安全区。
7. 背景音乐建议选择克制的低频电子氛围，90-100 BPM。节奏点可放在 1.8s、4.0s、6.2s、8.4s、10.8s、13.0s 和 15.0s。
8. 音效建议：1.8s 和 4.0s 使用轻微 magnetic click；6.2s 加入手指滑动声；8.4s 加入低声环境声；10.8s 加入键盘轻响；15.0s 留 0.4 秒尾响。
9. 前 3 秒必须出现完整产品；检查产品边缘、手机摄像头和手部是否被关键帧裁切。
10. 导出 H.264，1080 x 1920，30 fps。概念展示可使用 12-20 Mbps；面试 PDF 使用分镜静帧。

最终 FFmpeg 成品使用 `scene-assets/endcard-base.png` 作为第 07 镜头的无文字底图，再叠加一套完整品牌文案；`storyboards/07-endcard.png` 保留为原始分镜参考，避免重复品牌字样。

## 结尾画面

第 07 镜头为品牌收束画面，保留 `NOVAIR FluxDock` 和概念项目声明语境。不要添加未经验证的散热数字、性能排名、认证、销量或奖项。
