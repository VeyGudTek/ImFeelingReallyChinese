---
description: "Use when the user asks to save, add, log, export, or append Chinese vocabulary to a Markdown table. Handles Cantonese/Mandarin vocab entries with pinyin, jyutping, definitions, and examples."
tools: [read, edit]
---

## Vocabulary table behavior

When the user asks to save, add, log, export, or append vocabulary to a Markdown table:

1. Ask for the target Markdown file if it is not already specified.
2. If the target file does not exist, create it with this header:

   | Word | English definition | Mandarin | Cantonese |
   | --- | --- | --- | --- |

3. Add one row per vocabulary item.
4. Always use simplified Chinese characters.
5. In the **Word** column, use the Chinese word or phrase being learned.
   - If the written form is identical in Mandarin and Cantonese, list it once.
   - If Mandarin and Cantonese use different written forms, put the Mandarin form first, then `<br>`, then the Cantonese form (e.g., `吃饭<br>食饭`).
   - If a word exists in only one language (e.g., `咩`, `边度`), list that form and note the gap in the **English definition** column (e.g., "(Cantonese only; Mandarin: 什么)").
6. In the **English definition** column, provide a concise natural English definition.
7. In the **Mandarin** column, write a short, natural Mandarin example sentence that uses the word, then its English translation in parentheses, then Hanyu Pinyin with tone marks for the **entire example sentence** (not just the word) — each on its own line separated by `<br>`. If there is no Mandarin example, give the word-level Pinyin instead.
8. In the **Cantonese** column, write a short, natural Cantonese example sentence that uses the word, then its English translation in parentheses, then Cantonese Jyutping with tone numbers for the **entire example sentence** (not just the word) — each on its own line separated by `<br>`. If there is no Cantonese example, give the word-level Jyutping instead.
   - If a word exists in only one language, fill only that language's column and leave the other column empty (or note the gap per rule 5).
9. Escape Markdown-table special characters such as `|` with `\|`.
10. Avoid duplicate entries. If the word already exists, update the existing row only if the new definition, pronunciation, or example is more useful.
11. Confirm which file was changed and show the added or updated table row.

### Vocabulary table example

| Word | English definition | Mandarin | Cantonese |
| --- | --- | --- | --- |
| 学习 | to study; to learn | 我每天学习中文。<br>(I study Chinese every day.)<br>Wǒ měitiān xuéxí Zhōngwén. | 我每日学习中文。<br>(I study Chinese every day.)<br>Ngo5 mui5 jat6 hok6 zaap6 Zung1 man4*2. |
| 吃饭<br>食饭 | to eat a meal | 我们吃饭吧。<br>(Let's eat.)<br>Wǒmen chīfàn ba. | 我哋食饭啦。<br>(Let's eat.)<br>Ngo5 dei6 sik6 faan6 laa1. |
| 咩 | what (Cantonese only; Mandarin: 什么) | 你说什么呀？<br>(What are you saying?)<br>Nǐ shuō shénme ya? | 你讲咩呀？<br>(What are you saying?)<br>Nei5 gong2 me1 aa3? |
