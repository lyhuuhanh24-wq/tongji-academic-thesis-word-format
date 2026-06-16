---
name: academic-thesis-word-format
description: Use this skill when editing Chinese academic Word documents that need thesis-style formatting, heading hierarchy cleanup, table of contents updates, WPS navigation outline repair, figure/table/formula formatting, reference formatting, or user-specified chapter structure optimization.
---

# Skill: Chinese Academic Thesis Word Formatting and Structure Optimization

## 1. Purpose

This skill is used to edit Chinese academic Word documents, including:

* Undergraduate thesis;
* Master’s thesis;
* Course paper;
* Research paper;
* Academic report;
* Thesis-style chapter draft.

The main tasks are:

1. Standardize Word document formatting;
2. Normalize heading styles and outline levels;
3. Repair or update the front table of contents;
4. Repair the WPS left-side navigation outline;
5. Format body text, abstracts, references, figures, tables, and formulas;
6. Remove or downgrade non-thesis-style modules;
7. Optimize the structure of a specific chapter only when explicitly requested by the user.

The default behavior is conservative: preserve the original academic content and only adjust formatting, styles, outline levels, and document structure.

---

## 2. Core Principles

When this skill is used, follow these principles:

1. Preserve the original academic meaning.
2. Do not rewrite, delete, or compress body text unless explicitly requested.
3. Do not modify chapters or sections outside the user-specified scope.
4. Do not introduce unsupported new arguments or concepts.
5. Do not overwrite the original Word file.
6. Save the edited result as a new `.docx` file.
7. Ensure the front table of contents matches the real heading hierarchy.
8. Ensure WPS left-side navigation only displays formal academic headings.
9. Ensure body paragraphs, list items, captions, examples, and explanatory notes do not enter the WPS navigation pane.
10. Remove or convert non-thesis-style modules when the task is to create or normalize a thesis-style document.

---

## 3. Recommended Workflow

When editing a Word document, follow this workflow:

1. Inspect the document structure.
2. Identify existing headings, body text, abstracts, references, captions, tables, figures, formulas, and TOC.
3. Confirm the requested scope:

   * Full-document thesis formatting;
   * TOC and WPS navigation repair only;
   * A specific chapter or section;
   * Chapter structure optimization;
   * Formatting without content changes.
4. Remove or downgrade non-thesis-style modules if the document is being converted to a thesis-style format.
5. Apply formatting and style rules.
6. Repair heading styles and outline levels.
7. Update or regenerate the front table of contents.
8. Verify that WPS navigation only displays valid academic headings.
9. Save the result as a new `.docx` file.
10. Report what was changed and what was left unchanged.

---

## 4. Scope Control Rules

### 4.1 Full-document formatting

If the user requests full-document formatting, you may modify:

* Heading styles;
* Body text;
* Abstract;
* Keywords;
* Table of contents;
* Captions;
* Tables;
* Figures;
* Formulas;
* References;
* Appendix;
* WPS navigation outline.

Do not rewrite academic content unless requested.

### 4.2 Specific-chapter formatting

If the user requests only one chapter or section, only modify that part.

Do not modify unrelated chapters.

You may update the front table of contents because page numbers and heading hierarchy may change.

### 4.3 Structure optimization

Only optimize chapter structure when the user explicitly asks.

Allowed actions:

1. Merge logically overlapping headings;
2. Split overly long sections when necessary;
3. Demote or promote headings when logically appropriate;
4. Adjust heading names for academic clarity;
5. Add short transition sentences when needed;
6. Renumber headings within the modified scope;
7. Update TOC and WPS navigation after modification.

Forbidden actions:

1. Do not delete important academic content;
2. Do not substantially shorten the original chapter;
3. Do not change the core argument;
4. Do not modify unrelated chapters;
5. Do not introduce unsupported new concepts;
6. Do not turn body paragraphs into headings.

---

## 5. Non-Thesis-Style Content Rules

For a general academic thesis template, the following modules are usually not appropriate unless the user explicitly wants a textbook-style or teaching-material document:

* 学习目标
* 本章小结
* 思考题
* 练习题
* 教学目标
* 案例导入
* 课堂讨论
* 知识拓展
* 本章重点
* 本章难点
* 学习提示
* 教学案例
* 课后习题
* 章节导读

### 5.1 Default handling

If the user asks to convert the document into a thesis-style or academic-paper-style format:

1. Remove these module headings if they are clearly unrelated to thesis writing.
2. If their content contains useful academic arguments, integrate the useful content into nearby body paragraphs.
3. Do not let these module labels enter the TOC or WPS navigation.
4. Do not retain textbook-like labels unless the user explicitly asks.

### 5.2 If the user only asks to repair formatting

If the user does not ask to convert the document into thesis style, do not delete these modules automatically.

Instead:

* Set them as normal body text or custom emphasis style;
* Set outline level to Body Text;
* Exclude them from WPS navigation and TOC.

---

## 6. Table of Contents Formatting

### 6.1 TOC Title

The title “目录” must be formatted as:

* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

### 6.2 TOC Entries

TOC entries must be formatted as:

* Font: 宋体
* Size: 小四
* Line spacing: 18 pt
* Space before: 0 pt
* Space after: 0 pt
* Page numbers: right aligned

The TOC must be generated or updated based on real heading styles and outline levels.

Do not manually type a fake TOC unless automatic TOC generation is impossible.

---

## 7. Heading Formatting and Outline Levels

Only formal academic headings should receive heading styles and outline levels.

### 7.1 Chapter Heading

Examples:

```text
第 1 章 绪论
第 2 章 文献综述
第 3 章 理论基础
```

Format:

* Style: Heading 1 / 标题 1
* Outline level: Level 1 / 级别 1
* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

Spacing rule:

* There should be one character space between the chapter number and the chapter title.
* Example: `第 1 章 绪论`

---

### 7.2 First-Level Section Heading

Examples:

```text
1.1 研究背景
1.2 研究意义
2.1 国内研究现状
```

Format:

* Style: Heading 2 / 标题 2
* Outline level: Level 2 / 级别 2
* Font: 黑体
* Size: 小三
* Alignment: left
* Line spacing: single
* Space before: 24 pt
* Space after: 6 pt

Spacing rule:

* There should be one character space between the section number and the title text.
* Example: `1.1 研究背景`

---

### 7.3 Second-Level Section Heading

Examples:

```text
1.1.1 研究问题的提出
2.1.1 国外研究现状
3.1.1 核心概念界定
```

Format:

* Style: Heading 3 / 标题 3
* Outline level: Level 3 / 级别 3
* Font: 黑体
* Size: 四号
* Alignment: left
* Line spacing: single
* Space before: 12 pt
* Space after: 6 pt

Spacing rule:

* There should be one character space between the section number and the title text.
* Example: `1.1.1 研究问题的提出`

---

### 7.4 Lower-Level Headings

Avoid excessive heading levels.

Default recommendation:

* Use no more than three heading levels:

  * Chapter heading;
  * First-level section heading;
  * Second-level section heading.

If lower-level headings such as `1.1.1.1` are retained, ensure they do not clutter the TOC or WPS navigation.

---

## 8. Body Text Formatting

All normal body paragraphs must be formatted as:

* Style: Normal / 正文
* Outline level: Body Text / 正文文本
* Chinese font: 宋体
* English font: Times New Roman
* Size: 小四
* Alignment: justified / 两端对齐
* First-line indent: 2 Chinese characters
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt

Special notes:

* If a paragraph contains mathematical expressions, line spacing may be adjusted as needed.
* Body paragraphs must never use Heading 1, Heading 2, or Heading 3.
* Body paragraphs must never appear in the WPS navigation pane.

---

## 9. List and Numbered Paragraph Rules

Paragraphs beginning with list markers are usually body text, not headings.

Examples:

```text
（1）数据采集环节存在缺失
（2）数据处理规则不统一
（3）数据应用反馈机制不足
一是数据来源复杂
二是系统接口不稳定
三是人工录入存在误差
```

These paragraphs must be formatted as:

* Style: Normal / 正文
* Outline level: Body Text / 正文文本
* Chinese font: 宋体
* English font: Times New Roman
* Size: 小四
* Alignment: justified
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt

They must not appear in the WPS navigation pane.

Exception:

If the user explicitly wants list items to become formal headings, convert them carefully and consistently.

---

## 10. Abstract Formatting

### 10.1 Chinese Abstract Title

“摘要” title:

* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

### 10.2 Chinese Abstract Body

* Font: 宋体
* Size: 小四
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt
* First-line indent: 2 Chinese characters

### 10.3 Chinese Keywords

“关键词” paragraph:

* Font: 宋体
* Size: 小四
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt
* Bold only the label “关键词”.

---

## 11. English Abstract Formatting

### 11.1 English Abstract Title

“ABSTRACT” title:

* Font: Arial
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

### 11.2 English Abstract Body

* Font: Times New Roman
* Size: 小四
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt

### 11.3 English Keywords

“Key Words” paragraph:

* Font: Times New Roman
* Size: 小四
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt
* Bold only the label “Key Words”.

---

## 12. Figure, Table, and Formula Formatting

### 12.1 Figure Captions

Figure captions should be placed below figures.

Examples:

```text
图 3.2 非线性构形状态转移过程示意图
图 4.1 数据治理流程图
```

Format:

* Style: Normal, Caption, or custom Figure Caption style
* Outline level: Body Text / 正文文本
* Font: 宋体
* Size: 五号
* Alignment: center
* Line spacing: single
* Space before: 6 pt
* Space after: 12 pt

Spacing rule:

* There should be one character space between the figure number and the figure title.

Figure captions must not appear in the WPS navigation pane.

---

### 12.2 Table Captions

Table captions are usually placed above tables.

Examples:

```text
表 3.1 数据质量标准分类表
表 4.2 数据质量风险评估表
```

Format:

* Style: Normal, Caption, or custom Table Caption style
* Outline level: Body Text / 正文文本
* Font: 宋体
* Size: 五号
* Alignment: center
* Line spacing: single
* Space before: 6 pt
* Space after: 6 pt

Spacing rule:

* There should be one character space between the table number and the table title.

Table captions must not appear in the WPS navigation pane.

---

### 12.3 Formula Formatting

Formula formatting rules:

* Formula body: centered;
* Formula number: right aligned;
* Keep formula content unchanged;
* Keep formula numbering unchanged unless the user requests renumbering.

Example layout:

```text
                    formula content                         （3.1）
```

---

## 13. References Formatting

### 13.1 References Title

“参考文献” title:

* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

### 13.2 References Entries

* Chinese font: 宋体
* English font: Times New Roman
* Size: 五号
* Hanging indent: 2 characters
* Line spacing: 16 pt
* Space before: 0 pt
* Space after: 0 pt

Do not change reference content unless requested.

---

## 14. Appendix, Acknowledgements, and Academic Resume

### 14.1 Appendix

Appendix title should follow chapter heading style:

* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

Appendix body:

* Chinese font: 宋体
* English font: Times New Roman
* Size: 小四
* Alignment: justified
* First-line indent: 2 Chinese characters
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt

---

### 14.2 Acknowledgements

Acknowledgements title:

* Font: 黑体
* Size: 三号
* Bold: yes
* Alignment: center
* Line spacing: single
* Space before: 24 pt
* Space after: 18 pt

Acknowledgements body:

* Font: 仿宋
* Size: 小四
* Alignment: justified
* First-line indent: 2 Chinese characters
* Line spacing: 20 pt
* Space before: 0 pt
* Space after: 0 pt

---

### 14.3 Personal Resume and Academic Achievements

Title should follow chapter heading style.

Body:

* Chinese font: 宋体
* English font: Times New Roman
* Size: 五号
* Line spacing: 16 pt
* Space before: 0 pt
* Space after: 0 pt

Sub-labels such as “个人简历”“已发表论文”“待发表论文”“研究报告” may be bold.

---

## 15. WPS Navigation Pane Repair Rules

The WPS left-side navigation pane should only display real academic headings.

### 15.1 Allowed in WPS Navigation

Only the following content should appear:

| Content Type                 | Style            | Outline Level |
| ---------------------------- | ---------------- | ------------- |
| Chapter heading              | Heading 1 / 标题 1 | Level 1       |
| First-level section heading  | Heading 2 / 标题 2 | Level 2       |
| Second-level section heading | Heading 3 / 标题 3 | Level 3       |

### 15.2 Excluded from WPS Navigation

The following must be set to:

* Style: Normal / 正文
* Outline level: Body Text / 正文文本

Excluded content includes:

1. Normal body paragraphs;
2. Numbered list items beginning with “（1）”“（2）”“（3）”;
3. Explanatory paragraphs beginning with “一是”“二是”“三是”;
4. Figure captions;
5. Table captions;
6. Case descriptions;
7. Formula explanations;
8. English explanations;
9. Parenthetical explanations;
10. Non-thesis module labels such as “学习目标”“本章小结”“思考题”“练习题”;
11. Any bold paragraph that is not a formal numbered heading.

---

## 16. General Chapter Structure Optimization Method

Use this section only when the user explicitly asks to optimize the structure of a chapter or section.

### 16.1 Structure Diagnosis

Before editing, inspect the chapter and identify:

1. Whether there are too many headings at the same level;
2. Whether some headings overlap in meaning;
3. Whether some headings should be demoted to subheadings;
4. Whether the chapter follows a clear academic logic;
5. Whether the current order supports reader understanding;
6. Whether the chapter has a coherent beginning, development, and conclusion.

### 16.2 Common Academic Structure Patterns

Choose the structure that best fits the chapter content and user request.

#### Pattern A: Background - Problem - Method - Conclusion

Use when a chapter introduces a research problem or academic argument.

Possible structure:

```text
X.1 研究背景
X.2 问题提出
X.3 分析方法
X.4 本章结论
```

#### Pattern B: Concept - Theory - Framework - Application

Use when a chapter introduces a concept, theory, or analytical framework.

Possible structure:

```text
X.1 概念界定
X.2 理论基础
X.3 分析框架
X.4 应用分析
```

#### Pattern C: Problem - Cause - Evaluation - Improvement

Use when a chapter discusses risks, problems, defects, or management issues.

Possible structure:

```text
X.1 问题识别
X.2 原因分析
X.3 方法评估
X.4 改进路径
```

#### Pattern D: Literature - Review - Comment - Research Gap

Use when a chapter is a literature review.

Possible structure:

```text
X.1 国外研究现状
X.2 国内研究现状
X.3 文献评述
X.4 研究不足与启示
```

### 16.3 Heading Consolidation Rules

When a chapter has too many same-level headings:

1. Merge headings that discuss the same logical stage.
2. Keep 3–4 first-level section headings when possible.
3. Demote detailed subtopics to lower-level headings.
4. Do not force all chapters into the same structure.
5. Preserve the original academic meaning.
6. Add short transition sentences only when needed.
7. Ensure heading names are parallel and academically appropriate.
8. Ensure the final structure reads smoothly from beginning to end.

### 16.4 Renumbering Rules

After structure adjustment:

1. Renumber headings within the modified scope.
2. Ensure heading numbering is continuous.
3. Ensure lower-level heading numbers match parent headings.
4. Update cross-references if they refer to changed headings.
5. Update figure, table, and formula references only if necessary.
6. Update the front TOC and WPS navigation.

---

## 17. TOC and Navigation Update Rules

After any formatting or structural adjustment:

1. Update the front automatic TOC.
2. Keep the TOC title format unchanged.
3. Ensure page numbers are correct.
4. Ensure TOC hierarchy matches real heading styles.
5. Ensure normal body text, list items, captions, and case text do not enter the TOC.
6. Ensure the WPS navigation pane shows only formal academic headings.

Expected navigation structure:

```text
第 1 章 ×××
  1.1 ×××
    1.1.1 ×××
    1.1.2 ×××
  1.2 ×××

第 2 章 ×××
  2.1 ×××
  2.2 ×××

第 3 章 ×××
  3.1 ×××
    3.1.1 ×××
  3.2 ×××
```

Navigation must not show:

```text
（1）……
（2）……
普通正文句子
图 3.1 ……
表 3.1 ……
案例说明文字
英文解释
学习目标
本章小结
思考题
练习题
```

---

## 18. Quality Check Before Final Output

Before delivering the edited file, check:

1. Are the requested chapters modified correctly?
2. Are unrelated chapters unchanged?
3. Are heading styles and outline levels correct?
4. Does the TOC reflect the actual heading hierarchy?
5. Does WPS navigation show only real headings?
6. Are body paragraphs excluded from navigation?
7. Are figure and table captions excluded from navigation?
8. Are list items excluded from navigation?
9. Are non-thesis-style modules removed or downgraded when required?
10. Is the original academic content preserved unless rewriting was requested?
11. Is the new file saved without overwriting the original?

---

## 19. Final Output Requirements

Save the result as a new `.docx` file.

Use a clear filename based on the task, such as:

```text
原文件名_论文格式已统一.docx
原文件名_目录导航已修复.docx
原文件名_章节结构已优化.docx
原文件名_论文模板修改版.docx
```

Report back to the user with:

1. Output file name;
2. Modified scope;
3. Whether content was changed;
4. Whether non-thesis-style modules were removed or downgraded;
5. Whether the front TOC was updated;
6. Whether WPS navigation was repaired;
7. Any limitations or items requiring manual checking.
