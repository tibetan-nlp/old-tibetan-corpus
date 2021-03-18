# CG3 normalization
This is the CG3 grammar for normalizing Old Tibetan orthography so that it becomes more like Classical Tibetan and can thus be segmented, tagged, and analyzed using tools designed for Classical Tibetan.

To compile: ```cg-comp ot2ct.txt ot2ct.cg```

To run: ```vislcg3 -g ot2ct.cg -I otannals-vislcg.txt > otannals-normalized-vislcg.txt```

For more details, see [Word of VISL -> Constraint Grammar](https://visl.sdu.dk/constraint_grammar.html)
