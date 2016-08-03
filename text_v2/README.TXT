LaTeX šablona pro seminární a jiné práce, v1.0 (2011-05-29)
Tomáš Pikálek <tpikalek@gmail.com>, http://www.tpikalek.net

Tuto šablonu je možné použít pro psaní seminárních a jiných prací. Já ji například použil pro psané své SOČky Stavba amatérské difúzní mlžné komory.

SEZNAM SOUBORŮ
 - 00-Hlavicka			adresář obsahující titulní strany práce
 - 00-Hlavicka/Abstrakt.tex	abstrakt
 - 00-Hlavicka/Podekovani.tex	poděkování
 - 00-Hlavicka/podpis.png	naskenovaný podpis, pokud jej chcete mít ve své práci, jinak prázdný obrázek
 - 00-Hlavicka/Posudek.pdf	posudek na Vaši práci, většinou naskenovaný
 - 00-Hlavicka/Prohlášení.tex	prohlášení
 - 00-Hlavicka/Titulka.tex	titulní strana
 - 00-Hlavicka/Zadani.pdf	originální naskenované zadání práce
 - 00-Reference/Reference.bib	seznam použité literatury pro BibTeX
 - 00-Styly/Opakuj.sty		styl pro opakování některých matematických znaků na začátku řádku
 - 00-Styly/Reference.bst	styl pro použitou literaturu (BibTeX)
 - 00-Styly/Styly.sty		nastavení vzhledu dokumentu
 - Text.tex			hlavní soubor
 - Text.pdf			výstup
Dále jsou obsaženy soubory s textem a ukázkami, které přibližně ukazují i vhodnou strukturu práce.


ZAČÍNÁME
 - nejdříve si otevřete soubor Text.tex a zkuste jej přeložit (viz dále)
      - proběhne-li překlad bez problému, můžete začít s editací
      - zobrazí-li se během překladu chyba a ten neproběhne, chybu si nechte zobrazit a příslušné řádky příslušných souborů zkuste zakomentovat nebo upravit
 - v souboru Text.tex je třeba upravit:
      - \documentclass podle toho, zda tisknete oboustranně nebo jednostranně (lze udělat dodatečně)
      - jméno, název a typ práce apod. - tato oblast je viditelně ohraničena, generuje se z ní zejména titulní strana
      - načtené soubory - opět viditelně ohraničená oblast, obsahuje soubory s vlastním textem práce
      - přílohy - poslední viditelně ohraničení oblast, vkládá přílohy
 - je třeba upravit soubory 00-Hlavicka/Abstrakt.tex, 00-Hlavicka/Podekovani.tex
 - vložte originální zadání do souboru 00-Hlavicka/Zadani.pdf (případně jeho vložení ze souboru Text.tex smažte)
 - vložte posudek do souboru 00-Hlavicka/Posudek.pdf (případně jeho vložení ze souboru Text.tex smažte)
 - jestliže chcete měnit vzhled dokumentu, upravte soubor 00-Styly/Styly.sty


PŘEKLAD
 - šablona je optimalizována pro překlad pomocí PDFLaTeX, testováva byla v distribuci OpenSuSE 11.4
 - vždy překládejte pouze soubor Text.tex!
      - používáte-li program Texmaker, otevřete tento soubor a dejte Volby → Prohlásit současný dokument za hlavní dokument
      - překlad je třeba provést nejméně dvakrát, někdy i třikrát
 - po každé úpravě seznamu použité literatury (soubor 00-Reference/Reference.bib) je třeba spustit BibTeX
      - používáte-li program Texmaker, vyberte Nástroje → BibTeX (nebo klávesa F11)
      - poté je třeba opět nejméně dvakrát spustit překlad


PSANÍ SEZNAMU POUŽITÉ LITERATURY
 - použitá literatura je v souboru 00-Styly/Reference.bst
 - ve výchozím nastavení se zobrazí veškerá literatura v tomto seznamu, nejen ta citovaná
 - kvůli problémům s češtinou je třeba diakritiku u autora zadávat poněkud složitějí
      - háček \+x
      - čárka \'x
      - tedy např. Šťastný napíšeme jako \+S\+tastn\'y


DŮLEŽITÉ VĚCI K SAZBĚ
 - na každý obrázek a tabulku je nutné se v textu odkazovat
 - každá položka v seznamu literatury musí být v textu použita


POZNÁMKY
 - jestliže máte nastavený encTeX, je vhodné v souboru 00-Styly/Styly.sty povolit balík encvlna
 - v souboru 00-Styly/Styly.sty zkuste též povolit makro opakuj, v případě problémů jej vypněte
 - ve výstupním PDF souboru jsou aktivní odkazy, které jsou barevně označené, to se však nevytiskne


DOPORUČENÍ
 - pro začátečníky je na psaní v LaTeXu vhodný např. program TexMakerX
 - na jednoduché obrázky doporučuji program IPE, který s LaTeXem velmi dobře spolupracuje
 - pro zpracování výsledků měření a kreslení grafů je vhodný Gnuplot, použijte termínál epslatex


SEZNAM ZMĚN
v1.0
 - první verze šablony, vychází z mé práce SOČ


TODO
 - čeština v BibTeXu
 - integrovat další užitečná makra, zejména pro matematiku
 - dokumentace
 - více příkladů (obrázky, tabulky, grafy)
 - přehlednější hlavičky souborů