---
layout: default
title: Uzbek spellchecker
---

# Uzbek spellchecker

<!-- Authors -->
<div class="authors">
  <div>
    Murzintcev&nbsp;Nikita<sup>1</sup>
    &emsp;
    Allayarov&nbsp;Piratdin<sup>1</sup>
    &emsp;
    Yuldasheva&nbsp;Shahlo<sup>2</sup>
    &emsp;
    Kurbaniyazov&nbsp;Gulmurza<sup>2</sup>
    &emsp;
    Primbetov&nbsp;Abbaz<sup>3</sup>
  </div>
</div>

<div style="height: 1em"></div>

<!-- Affiliations -->
<div class="affiliations">
  <p><sup>1</sup> Tashkent State University of Economics, Uzbekistan</p>
  <p><sup>2</sup> Nukus State Pedagogical Institute, Uzbekistan</p>
  <p><sup>3</sup> Hunan University, China</p>
</div>
<div style="height: 1em"></div>

<!-- Links -->
<div
  style="
    display: flex;
    justify-content: center;
    gap: 0.5em 1em;
    flex-wrap: wrap;
  "
>
  <a href="https://github.com/uzbek-spell/spellchecker" target="_blank">
    <button>
      <i class="ti ti-brand-github"></i>
      GitHub
    </button>
  </a>
  <a href="https://arxiv.org/abs/" target="_blank">
    <button>
      <i class="ti ti-article"></i>
      arXiv
    </button>
  </a>
  <script type="text/javascript">
    function toggleBibtex() {
      const $bibtex = $("#bibtex");
      $bibtex.css(
        "display",
        $bibtex.css("display") === "none" ? "block" : "none",
      );
    }
  </script>
  <a onclick="toggleBibtex()">
    <button>
      <i class="ti ti-book-2"></i>
      BibTeX
    </button>
  </a>
</div>

<section id="bibtex" style="display: none">
  <div style="height: 1em"></div>
  <div style="height: 1em"></div>
  <p>
    <code>
      Waiting for publication…
    </code>
  </p>
</section>

<div style="height: 1em"></div>


## Overview

  This page represents results of the research intended for development of general NLP tools and spellchecking software for Uzbek language. In the [repository](https://github.com/uzbek-spell/spellchecker/releases), you can find files in Hunspell format and an add-on for MS Office. Read the paper for description of Uzbek morphology.


## Install

**Warning:** the provided software is a proof of concept, and it is not recommended for end-users.

[Download](https://github.com/uzbek-spell/spellchecker/releases) and install add-on for Microsoft Office. Use it as a usual proofing tool. The software was tested for compatibility with Windows versions of MS Office 2016-2019 64-bit.

To add Uzbek language spellcheking to the applications supporting Hunspell dictionaries, such as LibreOffice, copy two files `uz_Latn_UZ.aff` and  `uz_Latn_UZ.dic` to the next folders:

- Linux: `/usr/share/hunspell`
- MacOS: `~/Library/Spelling`

Some applications could require additional steps, see the corresponding documentation. For example, [Adobe InDesign](https://helpx.adobe.com/indesign/kb/add_cs_dictionaries.html).


## Lemmatization and PoS-tagging

The provided dictionaries are fully compatible with Hunspell, and can be used with standard tools or incorporated into the code (see [supported interfaces](http://hunspell.github.io/)).

[Download](https://github.com/uzbek-spell/spellchecker/releases) two files `uz_Latn_UZ.aff` and  `uz_Latn_UZ.dic`, and execute the following examples:

Interactive analyzes providing lemmas and morphological information:

```
> hunspell -d uz_Latn_UZ -m
```

Lemmatization:

```
> hunspell -d uz_Latn_UZ -s
```


## Acknowledgements

This material is based upon work supported by the Modernizing Uzbekistan National Innovation System (MUNIS) project under Grant REP-2/6 in 2022-2024 years.

<div style="font-size: 0.8em">
This website template was adapted from Brent Yi's project page for <a href="https://brentyi.github.io/tilted/">TILTED</a>.
</div>
