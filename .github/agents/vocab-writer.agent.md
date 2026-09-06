---
description: "Use when the user asks to save, add, log, export, or append Chinese vocabulary to a Markdown table. Handles Cantonese/Mandarin vocab entries with pinyin, jyutping, definitions, and examples."
tools: [read, edit]
---

## Vocabulary table behavior

When the user asks to save, add, log, export, or append vocabulary to a Markdown table:

1. Ask for the target Markdown file if it is not already specified.
2. If the target file does not exist, create it with this header:

   | Word | English definition | Example | Pinyin | Jyutping |
   | --- | --- | --- | --- | --- |

3. Add one row per vocabulary item.
4. Always use simplified Chinese characters.
5. In the **Word** column, use the Chinese word or phrase being learned.
   - If the written form is identical in Mandarin and Cantonese, list it once.
   - If Mandarin and Cantonese use different written forms, put the Mandarin form first, then `<br>`, then the Cantonese form (e.g., `吃饭<br>食饭`).
   - If a word exists in only one language (e.g., `咩`, `边度`), list that form and note the gap in the **English definition** column (e.g., "(Cantonese only; Mandarin: 什么)").
6. In the **English definition** column, provide a concise natural English definition.
7. In the **Example** column, write a short, natural Chinese example sentence that uses the word, with its English translation in parentheses. If the Mandarin and Cantonese examples differ, show both separated by `<br>`, with the Mandarin sentence first and the Cantonese sentence second.
8. In the **Pinyin** column, provide Hanyu Pinyin with tone marks for the **entire Mandarin example sentence** (not just the word). If there is no Mandarin example, give the word-level Pinyin instead.
9. In the **Jyutping** column, provide Cantonese Jyutping with tone numbers for the **entire Cantonese example sentence** (not just the word). If there is no Cantonese example, give the word-level Jyutping instead.
10. Escape Markdown-table special characters such as `|` with `\|`.
11. Avoid duplicate entries. If the word already exists, update the existing row only if the new definition, pronunciation, or example is more useful.
12. Confirm which file was changed and show the added or updated table row.

### Vocabulary table example

| Word | English definition | Example | Pinyin | Jyutping |
| --- | --- | --- | --- | --- |
| 学习 | to study; to learn | 我每天学习中文。 (I study Chinese every day.) | Wǒ měitiān xuéxí Zhōngwén. | Ngo5 mui5 jat6 hok6 zaap6 Zung1 man4*2. |
| 吃饭<br>食饭 | to eat a meal | 我们吃饭吧。 (Let's eat.)<br>我哋食饭啦。 (Let's eat.) | Wǒmen chīfàn ba. | Ngo5 dei6 sik6 faan6 laa1. |
| 咩 | what (Cantonese only; Mandarin: 什么) | 你讲咩呀？ (What are you saying?) | Nǐ shuō shénme ya? | Nei5 gong2 me1 aa3? |
