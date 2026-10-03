# 图片来源与范围

全部图片均为 AI 生成的校准样本，**不是摄影师 Pablo Bueno 的摄影作品**。

| 文件 | 来源 | 用途 |
| --- | --- | --- |
| skills/dark-canvas/assets/calibrated-ochre-canvas.jpg | 2026-10-02 `image_gen`，暖金夕照色域 | 色域校准：暖金 |
| skills/dark-canvas/assets/calibrated-dusk-blue.jpg | 同日 `image_gen`，冷蓝夜渡色域 | 色域校准：冷色 + 单一暖色锚点 |
| skills/dark-canvas/assets/calibrated-morning-cream.jpg | 同日 `image_gen`，清晨薄雾色域 | 色域校准：奶白暖光 + 灰绿 |
| skills/dark-canvas/assets/calibrated-night-mono.jpg | 同日 `image_gen`，烟灰单色色域 | 历史单色近似样本，有色偏和旋涡笔触 |
| skills/dark-canvas/assets/calibrated-neutral.jpg | 上一轮 `image_gen`，旧中性灰配方 | 中性灰近似参考，非所有主题的默认 |
| skills/dark-canvas/assets/calibrated-monochrome.jpg | 上一轮 `image_gen`，烟灰单色变体 | 历史对照 |
| skills/dark-canvas/assets/accepted-landscape.jpg | 用户已有 Creative OS AI 生成案例 | 校准层次与表面 |
| skills/dark-canvas/assets/accepted-botanical.jpg | 用户已有 Creative OS AI 生成案例 | 校准植物剪影与留白 |
| examples/transfer-canvas.jpg | 2026-10-02 `image_gen` 编辑 `transfer-source.jpg` | 亚麻油画转换实测 |
| examples/transfer-source.jpg | 上一轮 `image_gen`，AI 合成普通照片式输入 | 转换输入，**非真实拍摄照片** |
| examples/legacy-neutral-recipe.jpg | 2026-10-02 `image_gen`，复现旧中性灰配方 | 旧配方对照 |
| examples/generate-cloud-bird.jpg | 上一轮 `image_gen`，旧暖灰从零生成 | 历史对照，场景有偏差 |
| examples/transfer-dark-canvas.jpg | 上一轮 `image_gen` 转换 | 历史对照，天空重绘偏差 |
| examples/transfer-neutral.jpg | 上一轮 `image_gen` 转换 | 历史对照，云形重绘偏差 |

## 权利说明

MIT 许可证适用于本仓库的原创文字与配置。**不表示第三方摄影作品被重新许可。** 仓库图片是 AI 生成样本，不是第三方摄影原图的复制或裁切。部分历史样本与参考的构图相近，不作为新构图能力的证明。

用户提供的摄影参考保存在被 Git 忽略的本地目录，**不随仓库与发布包分发**。小红书分享链接的临时参数（`xsec_token`、`shareRedId` 等）已全部剔除，只保留稳定主页地址。原始 Creative OS 文件未被改动。

## 宿主与原始输出

历史样本中有 WorkBuddy「AI生成」标识，予以保留。这个观察不证明所有宿主或所有 image_gen 输出都会压印水印；实际成图须逐张查看记录。当前 Codex 测试使用内建 image_gen，原始 PNG 保留在本地及公开测试目录，不作水印擦除。

历史 JPEG 为原始 PNG 的压缩版本，画面未因本次文档修订而更改。新增样本为 2026-10-03 Codex 内建 image_gen 实际输出：`examples/adaptive/street-v1/v2.png`（街道两版）、`stilllife-v1/v2/v3.png`（静物三版）、`portrait-v1/v2.png`（AI 虚构人物两版）。命名中的斜线表示各独立文件的版本，原始 PNG 未修改。湖面真实照片及两版转换均仅本地保存；公开记录不分发这些图片。

新增样本是候选成果，用户尚未作视觉验收；特别是人物诗意表达仍只部分达成。

## v0.4.1 平静布面候选

2026-10-03 Codex 内建 image_gen 编辑现有 AI 生成场景：`examples/flat-canvas/street-v1.png`、`street-v2.png`、`stilllife-v1.png`、`stilllife-v2.png`、`stilllife-v3.png`。均为原始 PNG，未作后期纹理处理；摄影参考只借平缓布面语言，未纳入仓库。真实湖面及三版转换只保存在本地。当前候选的装饰性细纹仍有偏差，标为部分达成，用户尚未视觉认可。
