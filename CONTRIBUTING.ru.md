# Содействие

🎌
[Čeština][CZ],
[Deutsch][DE],
[English][EN],
[Español][ES],
[Français][FR],
[Italiano][IT],
[Kurdi][KU],
[Lietuvių][LT],
[Nederlands][NL],
[Norsk][NO],
[Polski][PL],
[Português][PT_BR],
**Русский**,
[Türkçe][TR],
[Ελληνικά][GR],
[العربية][AR],
[日本語][JA],
[正體中文][ZH_TW],
[简体中文][ZH_CN],
[한국어][KO_KR]

[AR]:CONTRIBUTING.ar.md
[CZ]:CONTRIBUTING.cz.md
[DE]:CONTRIBUTING.de.md
[EN]:CONTRIBUTING.md
[ES]:CONTRIBUTING.es.md
[FR]:CONTRIBUTING.fr.md
[GR]:CONTRIBUTING.gr.md
[IT]:CONTRIBUTING.it.md
[JA]:CONTRIBUTING.ja.md
[KO_KR]:CONTRIBUTING.ko_kr.md
[KU]:CONTRIBUTING.ku.md
[LT]:CONTRIBUTING.lt.md
[NL]:CONTRIBUTING.nl.md
[NO]:CONTRIBUTING.no.md
[PL]:CONTRIBUTING.pl.md
[PT_BR]:CONTRIBUTING.pt_br.md
[RU]:CONTRIBUTTING.ru.md
[TR]:CONTRIBUTING.tr.md
[ZH_CN]:CONTRIBUTING.zh_cn.md
[ZH_TW]:CONTRIBUTING.zh_tw.md

Исходный код в этом репозитории был оцифрован вручную с бумажных распечаток, поэтому опечатки и другие расхождения внесены случайно. Код должен быть изменен для соответствия с представленными ниже отсканированными распечатками:

- [AGC printouts for Comanche][8]
- [AGC printouts for Luminary][9]

## Полезные расширения

GitHub имеет поддержку синтаксиса встроенного языка ассемблера AGC. К сожалению, Ваш редактор кода его не поддерживает, однако есть расширения для языка AGC, которые обеспечивают подсветку синтаксиса в следующих редакторах:

- [Atom][Atom]†
- [CodeBlocks][CodeBlocks]
- [Eclipse][Eclipse]
- [Kate][Kate]
- [ProgrammersNotepad][ProgrammersNotepad]
- [Sublime Text 3][Sublime Text]†
- [TextPad][TextPad]
- [Vim][Vim]
- [Visual Studio Code][VisualStudioCode]†
- [jEdit][jEdit]

† Поддерживает автоматическое форматирование

[Atom]:https://github.com/Alhadis/language-agc
[CodeBlocks]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/CodeBlocks
[Eclipse]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/Eclipse
[Kate]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/Kate
[ProgrammersNotepad]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/ProgrammersNotepad
[Sublime Text]:https://github.com/jimlawton/AGC-Assembly
[TextPad]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/TextPad
[Vim]:https://github.com/wsdjeg/vim-assembly
[VisualStudioCode]:https://github.com/wopian/agc-assembly
[jEdit]:https://github.com/virtualagc/virtualagc/tree/master/Contributed/SyntaxHighlight/jEdit

## Форматирование

**Примечание:** GitHub и расширения упомянутые выше обеспечат автоматическое использование правильного форматирования.

- Используйте табуляцию
- Ширина табуляции равна 8
- Удаляйте пробелы в конце строк

## Что я должен проверять?

Любые расхождения между сканами и исходным кодом в репозитории.

### Комментарии

Комментарии в транскрибированном коде **ОБЯЗАНЫ В ТОЧНОСТИ** соответствовать сканам.

Типичные ошибки на которые следует обратить внимание включают, но не ограничиваются:

#### Типографические ошибки

В некоторых местах, первичные разработчики делали типографические ошибки во время написания комментариев. Некоторые из них были ошибочно исправлены в процессе оцифровки, однако оцифровывание также должно отображать типографические ошибки которые не присутствуют на сканах.

На пример, если оцифрованный комментарий содержит `SPACECRAFT`, но в сканах было напечатано `SPAECRAFT`, то в оцифрованный комментарий **ОБЯЗАН** быть исправлен на `SPAECRAFT` (без `C`).

Также, если оцифрованное слово содержит опечатку, но в сканах ее нет, то опечатка **ОБЯЗАНА** быть исправлена.

#### Пробелы

Пробелы между двумя символами в комментариях **ДОЛЖНЫ** соответствовать сканам. В большинстве случаев (ознакомьтесь с обсуждением [#316][10]) это:

- Одинарный пробел для нового слова.
- Двойной пробел для нового предложения.
- Тройной пробел для отступа.

Не все страницы на сканах соответствуют этим правилам, если скан содержит один пробел вместо двух - используйте один.

### Разрывы строк

- Разрывы строк *содержащие* `R0000` в столбце 1 должны в точности соответствовать сканам.
- Разрывы строк *без* `R0000` в столбце 1 должны содержать только 1 или 2 пустые строки подряд.
  - Если более 2 пустых строк - уберите лишние разрывы строк.
    - Строки с `R0000` в столбце 1 не считаются пустыми.
  - В исходных изображениях они были созданы ненапечатанной цифрой в столбце 8. 2 принудительно использует двойной пробел (одна пустая строка), а 3 принудительно использует тройной пробел (две пустые строки). Значения 4-8 были определенны, но никогда не использовались. Читайте подробнее в [#159][7]

На пример:

```plain
R0819   SUBROUTINE TO SKIP...
R0820



 0821   LAMPTEST  CS  IMODES33
```

Должно быть изменено на:

```plain
R0819   SUBROUTINE TO SKIP...
R0820


 0820   LAMPTEST  CS  IMODES33
```

## Примечание

Перед созданием PR, пожалуйста, убедитесь, что Ваши изменения соответствуют сканам!

[0]:https://github.com/chrislgarry/Apollo-11/pull/new/master
[1]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[2]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[6]:https://github.com/wopian/agc-assembly#user-settings
[7]:https://github.com/chrislgarry/Apollo-11/issues/159
[8]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[9]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[10]:https://github.com/chrislgarry/Apollo-11/pull/316#pullrequestreview-102892741
