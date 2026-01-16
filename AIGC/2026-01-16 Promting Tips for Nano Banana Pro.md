---
title: "2026-01-16 Promting Tips for\_Nano Banana Pro"
tags: 新建,模板,小书匠
category: /小书匠/日记/2026-01
grammar_cjkRuby: true
---


核心逻辑： 不同于 Midjourney 的"咒语堆砌"，Nano Banana Pro (Gemini 3 Pro Image) 强调用结构化自然语言来控制画面。 本指南基于官方 "7 Promting Tips" 整理，专注于画面结构与物理属性的精准控制。
🏗️ 一、 完整架构：11维控制矩阵 (The 11-Dimensional Matrix)
1. 👨‍🎨 Subject (主体)
W (Who): 对象、外貌、数量。
P (Personality): 身份、性格、表情。
2. 📐 Composition (构图)
F (Frame): 景别（大特写/全身/极远景）。
A (Angle): 机位（上帝视角/蚂蚁视角/过肩镜头）。
S (Space): 留白位置（为文字预留顶部/左侧）。
3. 🏃 Action (动作)
Dynamic: 正在做什么？速度感如何？
Interaction: 和环境/物体的交互。
4. 📍 Location (场景)
Env: 地点、自然元素、建筑结构。
Atmosphere: 物理氛围（雾/烟/破碎）。
5. 💡 Camera & Lighting (光影)
注意：这里从 Style 里独立出来了，因为 Nano Banana Pro 能模拟物理摄影台。
Lens: 焦段 (16mm / 85mm / Macro)。
Light: 光位 (逆光/伦勃朗光) + 色温 (冷/暖)。
DOF: 景深控制 (f/1.2 虚化 / f/16 全清)。
6. 🎨 Style (风格)
Art: 媒介 (水彩/3D/油画/胶片)。
Color: 配色方案 (莫兰迪/赛博霓虹/黑白)。
Texture: 材质感 (粗糙纸张/光滑陶瓷)。
7. 🔠 Typography (文本排版) ★核心杀手锏
Text: 具体写什么字？ "Quote here"
Font: 字体风格 (手写/衬线/未来感)。
Pos: 放在哪？ (嵌入物体表面/悬浮在空中)。
8. 🧠 Factual Constraints (事实约束)
Gemini 3 Pro 特有能力。
Logic: "确保解剖学正确" / "符合 1980 年代历史细节" / "科学准确的剖面图"。
9. 🖼️ Reference Images (参考图逻辑)
Role: 图 A 做姿势，图 B 做画风，图 C 做背景。
多图工作流必备。
10. 🚫 Constraints (规则限制)
Negative: 禁止出现什么？ (无字/无人/无虚化)。
Hard Rules: "不得改变主角发型"。
11. 📤 Output Specs (输出规格)
Ratio: 9:16 (竖屏) / 16:9 (横屏)。
内容：要写什么字？ -> text "HELLO WORLD"
位置：写在哪？ -> written on a neon sign in the background
风格：什么字体？ -> in bold futuristic sans-serif font, glowing blue
示例：
A cyberpunk street scene, heavy rain. A neon sign hanging above a noodle shop says "NOODLES" in bright red kanji font. (赛博朋克雨夜街道。面馆上方挂着霓虹招牌，用鲜红汉字写着"NOODLES"。)
🧩 四、 多图与一致性 (Multi-Image & Consistency)
1. 角色一致性 (Character Consistency)
指令：Use [Image A] as the character reference.
控制：上传一张参考图，要求模型保持人物面部特征不变，但改变动作或场景。
2. 风格迁移 (Style Transfer)
指令：Use [Image B] for the art style.
控制：上传一张风格参考图（比如梵高画、皮影戏），让模型学习其笔触和配色。
3. 构图参考 (Pose/Composition Reference)
指令：Use [Image C] for the pose/composition.
控制：上传一张线稿或照片，要求模型严格遵照其构图结构。
🛠️ 五、 局部编辑 (In-painting / Editing)
生成完图后，使用 Edit 功能进行微调：
指令：Change the background to a snowy mountain. (把背景换成雪山)
指令：Add a pair of glasses to the character. (给角色加一副眼镜)
指令：Make the lighting warmer. (把光线调暖)
🚀 总结：万能结构公式
[主体描述] + [环境描述] + [动作/状态] + [构图/镜头参数] + [光影/氛围] + [风格/渲染] + [文字指令(可选)]
Copyable Example:
Subject: A futuristic samurai robot made of white porcelain and gold kintsugi cracks. Action: Standing in a combat stance, holding a glowing katana. Location: In a misty bamboo forest at dawn. Composition: Low angle shot, wide angle lens, looking up at the hero. Lighting: Soft morning mist lighting, volumetric god rays penetrating the bamboo. Style: Hyper-realistic 3D render, Octane render, ethereal atmosphere. Text: The katana blade has the text "HONOR" glowing in blue.