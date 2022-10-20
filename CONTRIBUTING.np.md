# Contributing

🎌
[Čeština][CZ],
[Deutsch][DE],
**English**,
[Español][ES],
[Français][FR],
[Italiano][IT],
[Kurdi][KU],
[Lietuvių][LT],
[Nederlands][NL],
[Norsk][NO],
[Polski][PL],
[Português][PT_BR],
[Türkçe][TR],
[Ελληνικά][GR],
[العربية][AR],
[日本語][JA],
[正體中文][ZH_TW],
[简体中文][ZH_CN],
[한국어][KO_KR]
[नेपाली][NP]

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
[TR]:CONTRIBUTING.tr.md
[ZH_CN]:CONTRIBUTING.zh_cn.md
[ZH_TW]:CONTRIBUTING.zh_tw.md
[NP]:CONTRIBUTING.np.md

यस भण्डारमा स्रोत कोड कागज प्रिन्टआउटबाट म्यानुअल रूपमा डिजिटाइज गरिएको थियो, त्यसैले टाइपो र अन्य विसंगतिहरू गलत रूपमा प्रस्तुत गरिएको छ। कोडलाई निम्न स्क्यान गरिएका प्रिन्टआउटहरूसँग सुसंगत बनाउन परिमार्जन गरिनेछ:

- [AGC printouts for Comanche][8]
- [AGC printouts for Luminary][9]

## Useful Extensions

गिटहव सँग AGC असेंबली भाषाको लागि सिन्ट्याक्स समर्थन छ। दुर्भाग्यवश तपाईंको कोड सम्पादकले गर्दैन, यद्यपि त्यहाँ AGC भाषा विस्तारहरू छन् जसले निम्न सम्पादकहरूको लागि सिन्ट्याक्स हाइलाइटिङ प्रदान गर्दछ:

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

† स्वचालित ढाँचा समर्थन गर्दछ

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

## ढाँचा

**नोट:** गिटहव र माथि चिन्ह लगाइएका विस्तारहरूले सुनिश्चित गर्नेछ कि तपाइँ स्वचालित रूपमा सही ढाँचा प्रयोग गर्दै हुनुहुन्छ।

- ट्याब इन्डेन्टेसन प्रयोग गर्नुहोस्
- 8 को ट्याब चौडाइ प्रयोग गर्नुहोस्
- ट्रिम ट्रेलिङ व्हाइटस्पेस

## म के जाँच गर्छु?

यस भण्डारमा स्क्यान र स्रोत कोड बीचको कुनै विसंगति।

### टिप्पणीहरू

ट्रान्सक्राइब गरिएको कोडमा भएका टिप्पणीहरू **अनिवार्य** स्क्यानसँग **ठ्याक्कै** मिल्नुपर्छ ।

तपाईंले प्रमाणीकरण गर्दा हेर्नुपर्ने सामान्य समस्याहरू समावेश छन्, तर सीमित छैनन्:

#### टाइपोग्राफिक त्रुटिहरू

केही स्थानहरूमा, मूल विकासकर्ताहरूले टिप्पणीहरू लेख्दा टाइपोग्राफिक त्रुटिहरू गरे। यी मध्ये केही प्रारम्भिक डिजिटाइजेसनको क्रममा गल्तीले सच्याइएको थियो, तर डिजिटाइजेसनले टाइपोग्राफिक त्रुटिहरू पनि प्रस्तुत गरेको छ जुन स्क्यानहरूमा उपस्थित थिएनन्।

उदाहरणका लागि, यदि डिजिटाइज गरिएका टिप्पणीहरूमा `SPACECRAFT` समावेश छ, तर `SPAECRAFT` स्क्यानमा छापिएको थियो भने, त्यसपछि डिजिटाइजेसन लाई `SPAECRAFT` (हराएको `C`) मा **अनिवार्य** सच्याउनुपर्छ।

त्यसैगरी, यदि कुनै शब्दको डिजिटाइजेसनमा टाइपो छ तर स्क्यानमा सही हिज्जे लेखिएको छ भने टाइपो **सच्याउनुपर्छ।

#### खाली ठाउँहरू

टिप्पणीहरूमा दुई वर्णहरू बीचको खाली ठाउँहरू **अनिवार्य** स्क्यानहरूसँग मेल खानु पर्नेछ। धेरै जसो अवस्थामा (मा छलफल हेर्नुहोस् [#316][10]), यो हो:

- नयाँ शब्दहरूको लागि एकल ठाउँ।
- नयाँ वाक्यहरूको लागि डबल ठाउँ।
- इन्डेन्टेसनको लागि ट्रिपल स्पेस।

स्क्यानमा भएका सबै पृष्ठहरूले यो सामान्यीकरणलाई पछ्याउँदैनन्, यदि स्क्यानहरूमा डबल स्पेसको सट्टा एकल स्पेस मात्र छ भने, एकल स्पेस प्रयोग गर्नुहोस्।

### लाइन ब्रेकहरू

- स्तम्भ १ मा `R0000` सँगको रेखा विच्छेदहरू स्क्यानसँग ठ्याक्कै मिल्नुपर्छ।
- स्तम्भ १ मा `R0000` सँग लाइन विच्छेदमा पङ्क्तिमा १ वा २ खाली रेखाहरू मात्र समावेश हुनुपर्छ।
  - यदि त्यहाँ 2 भन्दा बढी खाली लाइन ब्रेकहरू छन् भने, अतिरिक्त लाइन ब्रेकहरू स्ट्रिप गर्नुहोस्.
    - स्तम्भ १ मा `R0000` भएका रेखाहरू यसमा गणना गर्दैनन्.
  - स्रोत तस्बिरहरूमा, यी स्तम्भ 8 मा छाप्न नसकिने अंकहरूद्वारा सिर्जना गरिएको थियो। A 2 त्यहाँ डबल स्पेस (एकल खाली रेखा) र 3 ले तीन ठाउँ (दोहोरो खाली रेखा) लाई बाध्य पारेको छ। मान 4-8 परिभाषित गरिएको थियो तर कहिल्यै प्रयोग गरिएन। यसको बारेमा थप पढ्नुहोस् [#159][7]

उदाहरणका लागि निम्न:

```plain
R0819   SUBROUTINE TO SKIP...
R0820



 0821   LAMPTEST  CS  IMODES33
```


बन्नु पर्छ:

```plain
R0819   SUBROUTINE TO SKIP...
R0820


 0820   LAMPTEST  CS  IMODES33
```

## नोट

तपाईंले PR बनाउनु अघि, कृपया तपाईंको परिवर्तनहरू स्क्यानहरूसँग मिल्दोजुल्दो छ भनी सुनिश्चित गर्नुहोस्!

[0]:https://github.com/chrislgarry/Apollo-11/pull/new/master
[1]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[2]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[6]:https://github.com/wopian/agc-assembly#user-settings
[7]:https://github.com/chrislgarry/Apollo-11/issues/159
[8]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[9]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[10]:https://github.com/chrislgarry/Apollo-11/pull/316#pullrequestreview-102892741
