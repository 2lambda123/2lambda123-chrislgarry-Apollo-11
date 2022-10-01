# Kontribusi

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
[Indonesia][ID_ID]

[AR]:CONTRIBUTING.ar.md
[CZ]:CONTRIBUTING.cz.md
[DE]:CONTRIBUTING.de.md
[EN]:CONTRIBUTING.md
[ES]:CONTRIBUTING.es.md
[FR]:CONTRIBUTING.fr.md
[GR]:CONTRIBUTING.gr.md
[IT]:CONTRIBUTING.it.md
[ID]:CONTRIBUTING.id.md
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

Kode sumber dalam repositori ini didigitalkan secara manual dari cetakan kertas, sehingga kesalahan ketik dan perbedaan lainnya telah diperkenalkan secara tidak sengaja. Kode harus dimodifikasi agar konsisten dengan hasil pindaian berikut:

- [AGC cetakan untuk Comanche][8]
- [AGC cetakan untuk Luminary][9]

## Ekstensi Berguna

GitHub memiliki dukungan sintaks untuk bahasa rakitan AGC bawaan. Sayangnya editor kode Anda tidak akan melakukannya, namun ada ekstensi bahasa AGC yang menyediakan penyorotan sintaks untuk editor berikut:

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

† Mendukung pemformatan otomatis

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

## Format

**Catatan:** GitHub dan ekstensi yang ditandai di atas akan memastikan Anda menggunakan pemformatan yang benar secara otomatis.

- Gunakan lekukan tab
- Gunakan lebar tab 8
- Pangkas spasi kosong

## Apa yang harus saya periksa?

Setiap perbedaan antara pemindaian dan kode sumber dalam repositori ini.

### Komentar

Komentar dalam kode yang ditranskripsikan **HARUS** cocok dengan pindaian **persis**.

Masalah umum yang harus Anda perhatikan saat pemeriksaan termasuk, tetapi tidak terbatas pada:

#### Kesalahan Tipografi

Di beberapa tempat, pengembang asli membuat kesalahan ketik saat menulis komentar. Beberapa di antaranya salah dikoreksi selama digitalisasi awal, namun digitalisasi juga menimbulkan kesalahan tipografi yang tidak ada dalam pemindaian.

Misalnya, jika komentar digital berisi `SPACECRAFT`, tetapi `SPAECRAFT` dicetak dalam pindaian, maka digitalisasi **HARUS** dikoreksi menjadi `SPAECRAFT` (`C` tidak ada).

Demikian juga, jika sebuah kata memiliki kesalahan ketik dalam digitalisasi tetapi dieja dengan benar dalam pemindaian, maka kesalahan ketik **HARUS** diperbaiki.

#### Spasi

Spasi antara dua karakter dalam komentar **HARUS** cocok dengan pindaian. Dalam kebanyakan kasus (lihat diskusi di [#316][10]), ini adalah:

- Satu spasi untuk kata-kata baru.
- Spasi ganda untuk kalimat baru.
- Tiga ruang untuk lekukan.

Tidak semua halaman dalam pemindaian mengikuti generalisasi ini, jika pemindaian hanya memiliki satu spasi, bukan spasi ganda, gunakan satu spasi.

### Jeda baris

- Pemisahan baris *dengan* `R0000` di kolom 1 harus sama persis dengan pindaian.
- Pemisahan baris *dengan**__out__* `R0000` di kolom 1 hanya boleh berisi 1 atau 2 baris kosong dalam satu baris.
   - Jika ada lebih dari 2 jeda baris kosong, hapus jeda baris tambahan.
     - Baris dengan `R0000` di kolom 1 tidak diperhitungkan.
   - Dalam gambar sumber, ini dibuat oleh digit yang belum dicetak di kolom 8. A 2 di sana memaksa spasi ganda (baris kosong tunggal) dan 3 memaksa spasi tiga (garis kosong ganda). Nilai 4-8 didefinisikan tetapi tidak pernah digunakan. Baca selengkapnya di [#159][7]

Misalnya berikut ini:

```plain
R0819   SUBROUTINE TO SKIP...
R0820



 0821   LAMPTEST  CS  IMODES33
```

Harus menjadi:

```plain
R0819   SUBROUTINE TO SKIP...
R0820


 0820   LAMPTEST  CS  IMODES33
```

## Catatan

Sebelum Anda membuat PR, pastikan perubahan Anda konsisten dengan scan!

[0]:https://github.com/chrislgarry/Apollo-11/pull/new/master
[1]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[2]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[6]:https://github.com/wopian/agc-assembly#user-settings
[7]:https://github.com/chrislgarry/Apollo-11/issues/159
[8]:http://www.ibiblio.org/apollo/ScansForConversion/Comanche055/
[9]:http://www.ibiblio.org/apollo/ScansForConversion/Luminary099/
[10]:https://github.com/chrislgarry/Apollo-11/pull/316#pullrequestreview-102892741
