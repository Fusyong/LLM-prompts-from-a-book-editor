---
book: <book> 丹麦儿童文学作家安徒生所写的童话故事集 </book>
style: <style> illustration in style of Disney's Frozen concept art meets Pixar, digital painting, vibrant colors, magical sparkles, crystal clear rendering, flowing lines, modern fairy tale aesthetic, cheerful atmosphere, inspired by Lisa Keene and Brittney Lee, child-friendly fantasy --style raw </style>
character_sheet_ar: <character_sheet_ar> 4:3 </character_sheet_ar>
---

![](十.svg)

我是一个儿童图书编辑，正在编辑一本给小学三年级学生阅读的、{book}。

我将每次给你提供这本故事书中的一篇故事，请你充当一位设计Midjourney prompt的专家，为这篇故事编写一套Midjourney prompts，以便让Midjourney生成一组插画。

让我们一步一步地完成这个任务：

1. 根据故事的长度估算需要多少张插画：
    1. 每篇故事都需要1张文首环境插画；
    2. 少于2000字的故事，需要1-2张文中场景插画；
    3. 2000-5000字的故事，需要2-3张文中场景插画；
    4. 超过5000字的故事，每增加2000字，增加1-2张文中场景插画。

2. 编写定义这篇故事的插画风格的prompt片段。我们已经把这本书的基础插画风格定义为{style}，可以直接使用这个风格作为本篇故事的插画风格；或者根据故事内容需要，在这个风格的基础上略微调整，作为本篇故事的插画风格。

3. 根据故事中的具体描述，为每一位重复出现的主要人物编写一个（或多个，如果有必要）角色形象prompt：
    1. 保留角色的名字，比如拇指姑娘；
    2. 根据故事指定角色的人种，比如北欧人；
    3. 根据故事描述人物时所用的词语定义这个人物的详细外貌特征、服装、发型、配饰等；
    4. 通过脸部表情和姿态展示角色的性格特征，尤其要突出活泼、快乐、惊喜、好奇、乐于交往、富有爱心、幽默等积极正面的性格特征；
    5. {style}, 或做必要的调整
    6. 指定绘制站立的全身三视图（ three views, namely the front view, the side view and the back view）
    7. 指定干净的背景（pure white background 或 solid light gray background）
    8. 设置宽高比为 --ar {character_sheet_ar}
    9. 设置 --v 模型版本 --q 2 等通用参数

4. 根据全篇故事，编写文首环境插画prompt：
    1. 根据故事描述人物时所用的词语定义故事的典型环境，如自然环境、建筑、天气、生物、物品等，给读者以视觉和情绪上的引导；
    2. 定义较为开阔的视野，给读者总体印象
    3. 不要出现清晰的人物形象
    4. {style}, 或做必要的调整
    5. 设置 --ar 宽高比、--v 模型版本 --q 质量等通用参数

5. 根据故事的情节，选择关键场景编写一组场景插画prompts：
    1. 这些场景应在故事中均匀分布，突出故事发展的重要节点
    2. 根据故事中的一段文字及其上下文所用的词语，定义场景的具体内容，包括：
        - 主要角色的动作和表情
        - 详细的环境和背景描述
        - 关键道具和细节
        - 场景中的光源位置和类型（如自然光、人工光等）
    3. 设计多样化的构图，并根据构图的需要相应地设置 --ar 宽高比（建议使用 3:4、4:3、1:1、2:3、3:2 等标准比例）
    5. 光线和氛围设定（如 morning light, dramatic lighting, soft ambient light 等）
    6. 景别和视角设定（如 close-up shot, wide shot, bird's eye view 等）
    7. {style}, 或做必要的调整
    8. 设置 --v 模型版本 --q 质量等通用参数
    9. 在各个场景之间，主要通过线索和细节（如道具、环境、小物品等）体现故事的连续性和发展变化

6. 编写prompt时要遵循Midjourney的prompt格式要求，并且要：
    1. 以英文编写prompt
        - 按内容、视觉控制（包括风格、光线、景别、视角等）、参数等类别分行表述
        - 避免使用Midjourney可能拒绝的词语，用中性、客观的描述代替
    2. 并附中文使用说明，提示可以调整prompt的哪些内容和参数，以获得更好的效果
    3. 使用markdown格式输出如下：

<output>

# {story_title} 插画prompts设计

## 1. 插画风格定义

```text
{style} or the style modified for this story
```

**使用说明：**
- 如何调整风格强度
- 如何微调特定描述
- 等等

## 2. 角色设定

### 2.1 {角色1名称}

```text
detailed character description,
the style,
full body turnaround (front, side, back views),
pure white background,
parameters
```

**使用说明：**
- 角色特征调整建议
- 姿势变化建议
- 可选的服装/配饰变化
- 等等

### 2.2 {角色2名称}
// ... 同上格式

## 3. 文首环境插画

```text
detailed environment description,
the style,
lighting, mood, perspective and viewpoint specifications,
parameters
```

**使用说明：**
- 环境元素调整建议
- 光照、景别、视角等视觉效果调整建议
- 等等

## 4. 场景插画系列

### 4.1 场景一：{场景简述}

**场景原文：**
> 相关故事片段引用

```text
character poses and expressions,
detailed scene description,
layout and framing specifications,
the style,
lighting, mood, perspective and viewpoint specifications,
parameters
```

**使用说明：**
- 角色姿势和表情调整建议
- 场景元素调整建议
- 构图和构图变化建议
- 光照、景别、视角等视觉效果调整建议
- 等等

### 4.2 场景二：{场景简述}

// ... 同上格式

</output>

