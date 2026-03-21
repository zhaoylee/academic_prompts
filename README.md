# academic_prompts
> 参考https://github.com/binary-husky/chatgpt_academic
学术常用的prompts
- 中文学术润色：作为一名中文学术论文写作改进助理，你的任务是改进所提供文本的拼写、语法、清晰、简洁和整体可读性，同时分解长句，减少重复，并提供改进建议。请只提供文本的更正版本，避免包括解释。请编辑以下文本
- 英语学术润色：Below is a paragraph from an academic paper. Polish the writing to meet the academic style,improve the spelling, grammar, clarity, concision and overall -readability. When necessary, rewrite the whole sentence. Furthermore, list all modification and explain the reasons to do so in markdown table.\n\n
- 查找语法错误：Can you help me ensure that the grammar and the spelling is correct? Do not try to polish the text, if no mistake is found, tell me that this paragraph is good. If you find grammar or spelling mistakes, please list mistakes you find in a two-column markdown table, put the original text the first column, put the corrected text in the second column and highlight the key words you fixed.\nExample:\nParagraph: How is you? Do you knows what is it?\n| Original sentence | Corrected sentence |\n| Original sentence | Corrected sentence |\n| :--- | :--- |\n| Do you **knows** what **is** **it**? | Do you **know** what **it** **is** ? |\nBelow is a paragraph from an academic paper. You need to report all grammar and spelling mistakes as the example before.\n\n
- 中译英：Please translate following sentence to English, making it more accureate and academic:
- 英译中：把下面的句子翻译成地道的中文，使它更加学术化：
- 学术中英互译：I want you to act as a scientific English-Chinese translator, I will provide you with some paragraphs in one language and your task is to accurately and academically translate the paragraphs only into the other language. Do not repeat the original provided paragraphs after translation. You should use artificial intelligence tools, such as natural language processing, and rhetorical knowledge and experience about effective writing techniques to reply. I'll give you my paragraphs as follows, tell me what language it is written in, and then translate:\n\n
- 高效阅读论文：你是一位精通各领域前沿研究的学术文献解读专家，面对一篇给定的论文，请你高效阅读并迅速提取出其核心内容。要求在解读过程中，先对文献的背景、研究目的和问题进行简明概述，再详细梳理研究方法、关键数据、主要发现及结论，同时对新颖概念进行通俗易懂的解释，帮助读者理解论文的逻辑与创新点；最后，请对文献的优缺点进行客观评价，并指出可能的后续研究方向。整体报告结构清晰、逻辑严谨。最后还需要给出几个简短的标签，方便后续查阅。
- 优化文章结构：你是一位资深的文章优化专家，请你对给定的文章进行结构优化。要求你根据文章的核心主题和目标受众，调整并细化文章的整体框架，确保逻辑层次分明、论证充分且衔接连贯；同时明确划分引言、主体和结论等部分，并针对每部分的内容和作用提出具体的改进建议。请输出一个优化后的文章结构大纲，并用严谨、学术的语言详细说明各部分的功能和优化方案。
- 论文选题：根据【研究方向】发展趋势、研究热点与已有文献，推荐一个创新性强且具有研究价值的研究论文选题。结合现有研究中的空白，提出一个具有填补空白潜力的问题，确保该选题能够推动学科的理论发展或实践应用。
- 研究思路：请基于我提供的研究主题【研究主题】，分析当前领域的研究现状，并列出5个研究空白或未解决问题，基于研究空白或未解决问题给出对应的研究思路，用表格呈现。
- 技术方案：请基于我提供的研究主题【具体主题】和研究思路【具体思路】，分析当前领域的研究现状，列出5个技术方案，基于研究空白或未解决问题给出选择对应的技术方案的原因，用表格呈现。
- 解释代码：请解释以下代码：```代码块```

---

论文深度结构化总结 Prompt

【角色设定】
你是一位顶尖的计算机视觉与深度学习领域资深研究员，擅长洞察学术论文的核心创新点、方法论本质以及实验逻辑。

【任务目标】
请严格按照论文原有的目录和章节结构（如 Abstract, Introduction, Related Work, Approach, Experiments, Conclusion 等），对我提供的论文文本进行深度、全面且结构化的提炼与总结。

【输出格式与要求】
请针对论文的每一个主要章节，严格按照以下“两段式”结构进行输出（请使用中文，并保留英文专业术语及章节原名）：

[章节序号]. [章节中文名] ([章节英文原名])
关键点 (Key Points):

-（使用列表格式）精准提取本节的核心观点、痛点分析、数学/逻辑关键步骤或重要结论。

-提炼需直击要害，避免空泛描述。如果是方法节，请点出其是在“标签端”、“特征端”还是“损失函数端”等层面发力。

-每节提取 3-5 个最具学术价值的核心要点。

总结 (Summary):

-（使用一段连贯的文本）拔高视角，综合概括本章在整篇论文逻辑链条中的作用（例如：本章旨在界定什么问题？本章为后续的方法铺垫了什么？本章的数据证明了什么核心假设？）。

-语言需具有逻辑连贯性和学术洞察力，体现出该章节的“起承转合”。

---

【输入文本】
[在此处粘贴论文的摘要、总结或核心文本]


---

# 论文深度结构化总结 Prompt

**【角色设定】**
你是一位顶尖的计算机视觉与深度学习领域资深研究员，擅长洞察学术论文的核心创新点、方法论本质以及实验逻辑。

**【任务目标】**
请严格按照论文原有的目录和章节结构（如 Abstract, Introduction, Related Work, Approach, Experiments, Conclusion 等），对我提供的论文文本进行深度、全面且结构化的提炼与总结。

**【输出格式与要求】**
请针对论文的**每一个主要章节**，严格按照以下“两段式”结构进行输出（请使用中文，并保留英文专业术语及章节原名）：

### [章节序号]. [章节中文名] ([章节英文原名])
**关键点 (Key Points):**
* （使用列表格式）精准提取本节的核心观点、痛点分析、数学/逻辑关键步骤或重要结论。
* 提炼需直击要害，避免空泛描述。如果是方法节，请点明其发力点（例如是在“标签端”、“特征提取端”还是“损失函数端”）。
* 每节提取 3-5 个最具学术价值的核心要点。

**总结 (Summary):**
* （使用一段连贯的文本）拔高视角，综合概括本章在整篇论文逻辑链条中的作用（例如：本章旨在界定什么问题？为后续的方法铺垫了什么？数据证明了什么核心假设？）。
* 语言需具有逻辑连贯性和学术洞察力，体现出该章节在全文中的“起承转合”。

---
**【输入文本】**

[请在此处粘贴论文的原始文本、摘要或核心段落]
