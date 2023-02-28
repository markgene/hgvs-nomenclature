# extension

## Definition

Extension: a sequence change extending the reference amino acid sequence at the N- or C-terminal end with one or more amino acids.

## Description

Format (**<font color="red">N-terminal</font>**):  **"prefix""Met1""ext""position_new_initiation_site"**,  e.g. p.Met1ext-5

**"prefix"**  =  reference sequence used  =  p.<br>
**"Met1"**  =  normal translation initiation site  =  Met1<br>
**"ext"**  =  type of change is an extension =  ext<br>
**"position_new_initiation_site"**  =  position new upstream translation initiation site =  -5

Format (**<font color="red">C-terminal</font>**):  **"prefix""Ter_position""new_amino_acid""ext""Ter""position_new_termination_site"**,  e.g. p.Ter110GlnextTer17

**"prefix"**  =  reference sequence used  =  p.<br>
**"Ter_position"**  =  normal translation termination site  =  Ter110<br>
**"new_amino_acid"**  =  amino acid encoded by variant termination codon  =  Gln<br>
**"ext"**  =  type of change is an extension =  ext<br>
**"Ter"**  =  termination codon = Ter / \*<br>
**"position_new_termination_site"**  =  position new downstream translation termination site =  17

## Notes

* all variants **should be** described at the DNA level, descriptions at the RNA and/or protein level may be given in addition
* **prefix** reference sequence accepted is "p." (protein).
* **extension** variants have been accepted on <font color="red">2012-08-31</font>.
* **predicted consequences**, i.e. without experimental evidence (no RNA or protein sequence analysed), should be given in parentheses, e.g. p.(Ter110GlnextTer17) or p.(\*110Glnext\*17).
* variants affecting the translation initiation site (Met1) activating an upstream (N-terminal) translation initiation site are described as [_deletion-insertion_](/recommendations/protein/variant/delins/), those activating a downstream (C-terminal)  initiation site as a [_deletion_](/recommendations/protein/variant/deletion/).
* **prioritisation**: (1) extension, (2) frame shift or deletion-insertion.
## Examples

* p.Met1ext-5: a variant in the 5' UTR activates a new upstream translation initiation site starting with amino acid Met-5: **NOTE**: modified from p.Met1ext<font color="red">Met</font>-5
* p.Met1_Leu2insArgSerThrVal: amino acid Met1 is changed to Val activating an upstream translation initiation site at position -4 (Met-4), insertion amino acids ArgSerThrVal between Mat1 and Leu2.: **NOTE**:    this variant is **not** described as an extension (p.Met1Valext-4) since Met1, part of the normal amino acid sequence, is changed
* p.Ter110GlnextTer17  (alternatively p.\*110Glnext\*17): a variant in the stop codon (Ter/\*) at position 110, changing it to a Gln-codon (a no-stop variant) and adding a tail of new amino acids to the protein's C-terminus, ending at a new stop codon (Ter/\*) at position 17
* p.Ter327Argext\*? (alternatively p.\*327Argext\*?): a variant in the stop codon (Ter/\*) at position 327, changing it to an Arg-codon and adding a tail of new amino acids of unknown length (position \*?) since the shifted frame does not contain a new stop codon.
## Discussion

!!! note "How are variants at the protein level called that directly affect the translation initiation (start) codon?"

    The variant is called <b>start-lost</b> variant, one of two types of a protein extension, an N-terminal extension. Note the difference with a <b>start-gained</b> variant where the start codon itself is not directly affected, another type of N-terminal extension.

!!! note "How are variants at the protein level called that directly affect the translation termination (stop) codon?"

    The variant is called a <b>no-stop</b> or <b>stop-lost</b> variant, one of two types of a protein extension, a C-terminal extension.

!!! note "<a name='noend'></a>How do I describe an extension when no new stop codon is reached?"

    Such variants are described using the format p.Ter789ArgextTer?, i.e. "<b>extTer?</b>" to indicate that no new termination codon is encountered.

!!! note "How should a variant in the 5'UTR be described that gives rise to a new translation initiation site?"

    Description at the DNA-level is like c.-23A>T (changing c.-25 caGggt c.-19 to caTggt, creating a new ATG-triplet). Description at the RNA-level is r.-23a>u and at the protein level p.(Met1ext-8), indicating the predicted protein sequence is an N-terminal extension with 8 amino acids.

!!! note "Should I describe a duplication in the translation termination codon (TGA to TGGA) as a frame shift or as an extension?"

    The variant extends the amino acid sequence at the C-terminal end and is therefore by definition an <b>extension</b>.