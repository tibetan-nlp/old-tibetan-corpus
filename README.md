# Old Tibetan Corpus
Here you will find linguistically analyzed Old Tibetan documents as well as tools for processing Old Tibetan text. We have taken these documents directly from the [Old Tibetan Documents Online](https://otdo.aa-ken.jp/) project.

The _Old Tibetan Annals_ and the _Old Tibetan Chronicle_ were given a lot of love and care as they passed through these stages of analysis:

1. First, the Wylie transliteration from OTDO was converted to Unicode Tibetan text.
1. Next, this plain Unicode text was converted to [VISL CG](https://visl.sdu.dk/cg3/single/#stream-vislcg) format using regular expressions, with each Tibetan "syllable" counting as a VISL CG word form.
1. The ```ot2ct``` constraint grammar was applied to the VISL CG input with the ```--trace``` flag enabled. This grammar eliminates the orthographic peculiarities of Old Tibetan, making it more similar to Classical Tibetan text.
1. The normalized text was then automatically word segmented and part-of-speech tagged using a tagger trained on Classical Tibetan materials.
1. The tagged text was converted to [BRAT standoff format](https://brat.nlplab.org/) for manual annotation.
1. In BRAT, incorrect segmentations and POS-tags were manually corrected. In addition, verb-argument and some other linguistic dependencies were annotated.
1. The text was then exported from BRAT standoff format to [CONLLU format](https://universaldependencies.org/format.html). As part of this process, the text was "denormalized" back to its original Old Tibetan orthographic practice using the debugging information output by the ```--trace``` flag.

In the case of the _Old Tibetan Annals_, we copied the English translation of the text from _The Old Tibetan Annals: An Annotated Translation of Tibet's First History_ by Brandon Dotson, and aligned this translation to the Tibetan text. You can see this in the CONLLU file for the text.

The _archive_ directory contains files in legacy or unmaintained formats.

You may cite this work by referencing this repository and its authors: Christian Faggionato, Edward Garrett, and Marieke Meelen. We thank the AHRC for its funding of the project _Lexicography in Motion_ (2017-2020, PI Ulrich Pagel).

Here is some metadata about the collection.

| Key | Value |
| ------------- | ------------- |
| Text ID | OTA |
| Title (eng) | Old Tibetan Annals |
| Title (bod) | -- |
| Source (eng) | Dotson, Brandon (2009). The Old Tibetan Annals: An Annotated Translation of Tibet's First History. VÖAW, Austria. |
| Source (bod) | https://otdo.aa-ken.jp/archives.cgi?p=Pt_1288 |
| Date | 25-07-2017 |
| Author | Unknown |
| Translation | Brandon Dotson |
| Tagging | Christian Faggionato, Marieke Meelen |
| Annotation | Christian Faggionato |
| Alignment | Christian Faggionato |
| Genre | History |
| Region | Tibet |
| Language | Tibetan, Old |
| Normalization | Yes |
| Licensing | Creative Commons Attribution 4.0 International License (CC-BY) |
| Annotator's notes | Regular grammatical structure, uniform verb frames, repetitive narrative structure. |

| Key | Value |
| ------------- | ------------- |
| Text ID | OTC |
| Title (eng) | Old Tibetan Chronicle |
| Title (bod) | -- |
| Source (eng) | Dotson, Brandon (2013). The Victory Banquet. The Old Tibetan Chronicle and the Rise of Tibetan Historical Narrative. Unpublished Habilitation script, Ludwig-Maximilians-Universität, München. |
| Source (bod) | https://otdo.aa-ken.jp/archives.cgi?p=Pt_1287 |
| Date | 08-08-2017 |
| Author | Unknown |
| Translation | -- |
| Tagging | Christian Faggionato, Marieke Meelen |
| Annotation | Christian Faggionato |
| Alignment | -- |
| Genre | History |
| Region | Tibet |
| Language | Tibetan, Old |
| Normalization | Yes |
| Licensing | Creative Commons Attribution 4.0 International License (CC-BY) |
| Annotator's notes | Prose interspersed with songs and poems, rich vocabulary, diverse verb structures - e.g. light verbs. |
