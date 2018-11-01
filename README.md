# TransliterationRuSiriShortcut
Transliteration from Russian


used `^(\D),.*\s(\w*)$` to get first and second group of table from [Wikipedia](https://ru.wikipedia.org/wiki/Транслитерация_русского_алфавита_латиницей)

then replaced with `<dict><key>WFWorkflowActionIdentifier</key><string>is.workflow.actions.text.replace</string><key>WFWorkflowActionParameters</key><dict><key>WFReplaceTextCaseSensitive</key><false/><key>WFReplaceTextFind</key><string>$1</string><key>WFReplaceTextReplace</key><string>$2</string></dict></dict>`

then added empty substitutions for Ъ and Ь

## Транслитерация русского Siri Shortcut

В качестве словаря замен взял табличку из [Википедии](https://ru.wikipedia.org/wiki/Транслитерация_русского_алфавита_латиницей).

Замену делаю без учёта регистра на последнее значение в табличке (кроме случая с Ъ и Ь - из заменяю на отсутствие символа).
