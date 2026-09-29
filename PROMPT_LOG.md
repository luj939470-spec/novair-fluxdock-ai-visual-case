# PROMPT LOG — NOVAIR FluxDock

## 0. 一致性基线

产品母版描述：compact magnetic smartphone cooler, rounded-square body, satin silver metal rim, deep graphite back plate, centered circular magnetic ring, one small pill-shaped side button, single USB-C port centered on the bottom edge, subtle radial vent detail, no logo, no text.

固定负面约束：no real brand, no logo, no trademark, no watermark, no text inside the image, no extra buttons, no extra ports, no visible wires unless requested, no impossible hinges, no floating parts, no duplicated product, no warped geometry, no excessive cyberpunk glow, no particles, no fake performance numbers.

## 1. 产品母版 / product-master

```text
Use case: product-mockup
Asset type: product consistency master sheet
Primary request: a clean industrial design master sheet for a fictional magnetic smartphone cooler named FluxDock, showing front, back, 45-degree, side, and attached-to-phone use state in one orderly board
Scene/backdrop: warm off-white studio background, generous spacing, neutral presentation board
Subject: compact rounded-square magnetic phone cooler; satin silver metal rim; deep graphite back plate; centered circular magnetic ring; one small pill-shaped side button; one centered USB-C port on bottom edge; subtle radial vent detail
Style/medium: premium 3D product visualization, realistic but presentation-ready
Composition/framing: five consistent views aligned in a grid; same exact object in every view; front, back, 45-degree, side, attached to a generic modern smartphone
Lighting/mood: soft studio light, controlled highlights, clean shadow
Color palette: off-white, graphite, satin silver, restrained cool blue accent
Materials/textures: anodized metal rim, matte polymer back, fine vent texture
Text (verbatim): none
Constraints: lock silhouette, button count, port location, ring position and materials across every view; no logo or typography
Avoid: no real brand, no watermark, no extra controls, no extra ports, no impossible geometry, no text, no neon clutter
```

Iteration: first pass prioritized a clear turntable and legible construction cues. Any generated labels are ignored and replaced by HTML labels in the case-study page.

## 2. Transparent product cutout

```text
Use case: background-extraction
Asset type: transparent-background product cutout
Primary request: a single FluxDock magnetic phone cooler, 45-degree front view, isolated on a genuinely transparent background
Subject: same product master; rounded-square graphite body, satin silver rim, centered magnetic ring, single side button, one bottom USB-C port
Style/medium: premium product photography / 3D render
Composition/framing: centered, full object visible, no crop, soft contact shadow only if it remains separate and subtle
Lighting/mood: soft cool studio lighting
Constraints: preserve exact master silhouette and materials; no text, no logo, no watermark
Avoid: additional buttons, extra ports, cables, phone, hands, glow, particles
```

## 3. 16:9 brand hero

```text
Use case: ads-marketing
Asset type: 16:9 ecommerce brand hero background
Primary request: premium international 3C campaign hero for a fictional magnetic phone cooler, with the product as the clear visual focus and generous negative space for manually typeset copy
Scene/backdrop: pale mineral tabletop and soft architectural shadow, clean studio environment
Subject: same FluxDock product master in a 45-degree hero view, aligned and physically plausible
Style/medium: photorealistic product campaign image
Composition/framing: product on the right third, open negative space on the left, wide 16:9 composition
Lighting/mood: soft directional morning light, calm, precise, premium
Color palette: warm white, graphite, satin silver, muted electric blue accent
Materials/textures: matte stone, anodized metal, subtle glass reflections
Text (verbatim): none; all copy added later in HTML
Constraints: product remains the visual subject, no logo, no text, no numerical claims
Avoid: cyberpunk overload, particles, fake UI, visible brand marks, product distortion
```

## 4. Square commerce image

```text
Use case: product-mockup
Asset type: 1:1 overseas ecommerce product image
Primary request: clean square product image of the same FluxDock magnetic phone cooler attached to a generic smartphone, showing the magnetic relationship clearly
Scene/backdrop: soft light grey studio gradient, no props
Composition/framing: centered product and phone, enough margin for overlay labels added later
Lighting/mood: soft top light with precise edge definition
Color palette: light grey, graphite, silver, small cool blue accent
Constraints: same product geometry; generic phone with no logo; no generated text
Avoid: real brand, extra buttons or ports, distorted phone, busy background, excessive glow
```

## 5. Social lifestyle trio

```text
Use case: photorealistic-natural
Asset type: campaign scene image set
Primary request: three restrained lifestyle scenes featuring the exact same FluxDock product master: a mobile gaming moment, a commuter seat moment, and a tidy desk-work moment
Scene/backdrop: 3-panel editorial contact sheet; gaming handheld atmosphere, train or cafe commute, minimal desk with laptop and notebook
Subject: same magnetic phone cooler attached to a generic smartphone; product readable in each panel
Style/medium: premium editorial product photography
Composition/framing: each panel has clear product visibility and quiet negative space; no faces required
Lighting/mood: gaming cool contrast, commute daylight, desk soft daylight; consistent premium treatment
Color palette: graphite, silver, warm white, muted electric blue
Constraints: no brand marks, no generated copy, no device UI text, no impossible hand anatomy, exact product consistency
Avoid: neon overload, particles, fake performance claims, recognizable real products
```

## 6. 9:16 cover

```text
Use case: ads-marketing
Asset type: 9:16 short-video cover background
Primary request: vertical campaign cover with the same FluxDock product floating slightly above a pale stone surface, calm premium tech mood, clear central silhouette and top/bottom safe areas for typeset copy
Composition/framing: product centered lower-middle, open top area, 9:16 portrait
Lighting/mood: soft directional light with cool blue reflected edge
Constraints: same product master; no text, no logo, no watermark, no particles
Avoid: busy background, product duplication, impossible geometry, excessive glow
```

## 淘汰方案

- 科技冷感：视觉识别清晰，但黑底和蓝光容易把产品带入同质化电竞/硬件语境；保留为方向探索，不作为主方向。
- 运动电竞：速度线与霓虹有传播力，但容易遮挡产品结构，且会稀释移动办公人群的覆盖；保留为社交广告备选。
- 极简国际化：产品识别最稳定，适合海外电商详情页与多尺寸适配；作为主方向。

## 三轮 Prompt 迭代证据

### Round 01 / Lock the object

先生成产品母版，明确圆角矩形轮廓、银色金属边、深石墨背板、中心圆环、单侧按键和底部 USB-C。目标是减少不同视角中的结构漂移。

### Round 02 / Shape the scene

在母版作为参考图的前提下，分别生成 16:9 主视觉、1:1 电商关系图、游戏 / 通勤 / 桌面三联场景和 9:16 封面。约束无文字、无 Logo，并为后续排版保留安全区。

### Round 03 / Verify the channel

筛选场景后，不再重新随机改变产品；用固定裁切和人工文字层适配 16:9、1:1、4:5、9:16。最终导出阶段检查标题字号、边缘、产品主体位置和每张图只保留一套文案。

## 人工调整记录

- 删除所有 AI 生成文字与伪 Logo，统一由 HTML/CSS 排版。
- 为商业图预留安全区，重新裁切为 16:9 / 1:1 / 4:5 / 9:16。
- 统一背景为 warm mineral / graphite / cool blue 色彩系统。
- 用 SVG 产品示意锁定轮廓、按键和接口的位置，作为页面内的结构说明。
- 检查反射、边缘、产品数量、手机连接关系与文字拼写。

## 可复用 Prompt 模板

```text
Use case: <taxonomy>
Asset type: <channel and ratio>
Primary request: <one visual objective>
Scene/backdrop: <environment>
Subject: SAME PRODUCT MASTER — rounded-square magnetic cooler, satin silver rim, deep graphite back, centered ring, one side button, one centered USB-C port
Style/medium: <photorealistic / 3D product visualization>
Composition/framing: <subject placement + safe areas>
Lighting/mood: <lighting>
Color palette: warm white, graphite, satin silver, muted electric blue
Text (verbatim): none; typeset later
Constraints: exact same silhouette and controls; no brand marks; no text; no impossible geometry
Avoid: <clutter, particles, over-glow, fake claims>
```

## 一致性检查清单

- [ ] 圆角矩形外轮廓一致
- [ ] 中央磁吸环位置一致
- [ ] 仅保留一个侧边按键
- [ ] USB-C 接口位于底部中央
- [ ] 银色金属边 + 深石墨背板材质一致
- [ ] 手机、手指和线缆关系物理可行
- [ ] 无真实品牌 Logo / 商标 / 伪 Logo
- [ ] 无 AI 乱码、虚假数字或无法证实的性能表述
- [ ] 文案由人工排版并完成拼写检查
- [ ] 输出比例与渠道安全区符合要求
