---
title: Gemini 3 Pro 落地页生成流程
summary: 用 Gemini 3 Pro 分五步生成高转化落地页的 6 条提示词模板：首屏定风格、图标动画细节、CTA、批量扩展板块
category: coding
tags: [Gemini-3-Pro, 落地页, 网页设计, 动画]
model: Gemini 3 Pro
source_name: 飞书 · Gemini 3pro 生成落地页
source_url: https://my.feishu.cn/wiki/LrsawphKHihfADkrw2TcHSJhnmf
collected: 2026-08-20
media: 0
---

# Gemini 3 Pro 落地页生成流程

> 用 Gemini 3 Pro 从 0 快速起草落地页的分步提示词：先用 50% 时间打磨首屏定下全站风格，再靠模板化提示词批量生成其余板块，最后人工精修。

## Prompt 原文

**第一步：生成首屏（附参考网站截图效果更好）**

```text
"为我的{应用类型}叫{名称}创建首屏,风格参考{参考网站}"
```

**第二步：指定 Iconify 图标集**

```text
"使用Iconify的{图标集名称}"
```

**第二步：逐元素入场动画**

```text
"逐元素添加淡入、滑入、模糊动画,使用'both'而非'forwards',不要用opacity 0"
```

**第三步：Logo 跑马灯动画**

```text
"为logo添加无限循环跑马灯动画,使用复制项和alpha遮罩"
```

**第三步：CTA 按钮（引用 UIVerse/Codepen 找的按钮代码）**

```text
"主按钮改为{代码},次级按钮改为{代码}。主按钮hover时添加1px边框光束动画"
```

**第四步：批量生成其他板块（附现有页面截图）**

```text
"适配新板块,修改文本、名称和数字"
```

## 来源

- 出处：[飞书 · Gemini 3pro 生成落地页](https://my.feishu.cn/wiki/LrsawphKHihfADkrw2TcHSJhnmf)
- 收录：2026-08-20

## 使用备注

- 原文是完整流程讲解，核心主张：AI 只是把 10 天压缩到 1 天，剩下的人工打磨才决定转化率。
- 五步流程：① 50% 时间花在首屏（导航栏/标题/副标题/CTA/社会证明/视觉元素），首屏定下全站颜色、字体、间距；② 细节：图标别用默认的，Iconify 有 Solar、HeroIcons、Iconoir、Phosphor 等几百个开源图标库，动画别让 AI 自由发挥；③ 社会证明放首屏或紧接着的位置，评级、品牌 logo 最好都放，CTA 按钮去 UIVerse 和 Codepen 找优质代码；④ 其他板块附截图批量生成，Gemini 3 会读取现有风格自动统一；⑤ 人工打磨：Midjourney 生成配图、Nano Banana Pro 混编风格、ChatGPT 优化文案。
- 背景动画可去 Unicorn Studio 找模板混编；Gemini 3 动画能力很强，可做光束、连接线等复杂动效。
