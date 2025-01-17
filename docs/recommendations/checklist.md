# Checklist

## Purpose

Going through publications one can easily see where people give variant descriptions that **do not correctly follow HGVS nomenclature**. The checklist below covers the most frequently offended rules. Going through should assist you while preparing a publication containing sequence variant descriptions.

## Checklist

1.  **Reference Sequence** - do you clearly mention the reference sequence used for numbering (nucleotides/amino acids) ?: A publication should mention, preferably in the Materials & Methods section and/or Figure or Table legend, which reference sequence file was used to describe variants and for numbering of the residues (DNA, RNA and protein (see [Reference Sequences](../background/refseq.md))).

    - Use a RefSeq accession with version number.
    - do not forget the underscore in the accession number (e.g., NM_004006.2).
    - genomic (g.) reference sequences start with nucleotide 1 and can not have nucleotides with additions like a +, - or \*.
    - for a coding DNA reference sequence, do you clearly state that nucleotide numbering starts with the A of the ATG translation initiation site as nucleotide 1 ?
    - legacy numbering is only allowed **in addition to** approved numbering
    - does your reference sequence contain the residue that you describe as changed ?
        - **NOTE**: NM reference sequences cover mature transcripts and do  not contain** intron and gene flanking sequences, and can only be used to describe variants in introns using a "c." prefix when a genomic reference sequence is given on which the coding DNA reference sequence is annotated, e.g. `NC_000023.10(NM_004006.2):c.94-2A>G` or `LRG_199t1:c.94-2A>G` (see [Reference Sequences](../background/refseq.md#DNAc))

2.  **Intronic variants** are descriptions of intron variants correct and complete ?

    - descriptions referring to exon or intron numbers instead of nucleotide positions, e.g."_c.IVS4-2A>G_", are **not allowed**.
    - do you properly describe ranges in the introns ? The format `c.123-65_123-50` is correct, the format `c.123-65**_-50**` is not, it is **incomplete**.

3.  **Insertions** - are descriptions of insertions correct and complete (see [Insertion](DNA/insertion.md))?

    - insertions should be reported using the format `c.51_52insT`.: The format `c.52insT` is **incomplete** and not allowed.
    - do you give the inserted sequence?: Describing a variant as `c.5439_5430**ins6**` is not allowed, the inserted sequence (for ins6 e.g. "TGCCAT") should be specified.
    - is the insertion reported indeed an insertion or is it in fact a duplication?: **Duplicating insertions** should be described as duplications, not as insertions (see [Duplication](DNA/duplication.md)).

4.  **The 3' rule** - do you correctly apply the 3' rule?: For deletions, duplications and insertions the **most 3' position possible is arbitrarily assigned** to have been changed (see [General recommendations](general.md)). This rule also applies to variants in single residue stretches (mono-nucleotide or amino acid) or tandem repeats.

5.  **Range** - the sign used to indicate a range is the "_" (underscore), not a "-" (minus)? The correct description to indicate a deletion of coding DNA nucleotides 12 to 14 is `c.12*14del`. Not correct is <code class="invalid">c.12-14del</code>, this describes a deletion of nucleotide -14 in the intron directly 5' of nucleotide `c.12` (see [Numbering](../background/numbering.md)).

6.  **Deletion** - do you indicate the first and last residue involved in a deletion? Descriptions like <code class="invalid">g.123del3</code> are not allowed, correct is `g.123_125del` (see [Deletion](DNA/deletion.md)).

7.  **Describe always at DNA-level** - do you describe all changes reported at DNA-level? All changes reported **must** be described at DNA-level

    - when descriptions at protein level are given in the text, upon first appearance, use a format like "`c.76G>T` (`p.(Gly26Cys)`, RNA not analysed)" or "`c.76G>T` (`r.76g>u` `p.Gly26Cys`)"

8.  **RNA level descriptions** HGVS nomenclature includes recommendations for the description of changes detected at the RNA level.

    - several transcripts derived from one allele are described using the format `r.[76a>c,73_88del]` (see [RNA](RNA/alleles.md))

9.  **protein level descriptions**

    - the protein reference sequence should represent the primary translation product, not a processed mature protein, and thus include the starting Methionine and a signal peptide sequence
    - the recommendation is to use **three letter amino acid code**
    - **"Ter" or "\*" should be used** to indicate a translation stop codon; the X should not be used
    - predicted "**silent**" protein level variants are described as **p.(Leu54=)**, not as _p.Leu54Leu_ or _p.54L/L_).
    - the description `p.(Met1Val)` is not allowed (see [Protein](protein/substitution.md))

10. **Mutation / polymorphism** Do not use the terms "mutation" or "polymorphism" (see [General recommendations](../background/basics.md))

    - "polymorphic" variants should not be described using the "/" (slash), describe them as normal variants like `c.127A>G` and `p.(Ile43Val)`.

11. **Recessive diseases** - do you clearly describe which changes are found in which combination? A publication describing variants in patients suffering from a recessive phenotype should, for each individual, explicitly mention **which variants were found and in which combination (per allele)**.

12. **Tabular overview** - is the overview of all changes reported clear and complete?: Preferably, a publication contains a **tabular overview** of all variants reported. This overview contains columns describing the change at the DNA-level (**absolutely essential**) and, optional, at the RNA and protein level.: When data on RNA and/or protein level are provided, it should be made clear whether the data were **deduced or experimentally verified** (i.e. state explicitly when RNA was analysed, e.g. to study the consequences of a variant affecting splicing).: Make sure **predicted** consequences at protein level are reported in parentheses, like `p.(Arg123Ser)`.

13. **Variant types**: When giving numbers regarding the types of variants identified do **not mix numbers** at DNA, RNA and protein level. Give numbers separately for DNA, RNA and protein. Where would you list a substitution at DNA level, giving a deletion at RNA level (since it affects splicing) and a frameshift at protein level?

14. **Pathogenic** Be careful when using the term "pathogenic" (see [General recommendations](../background/basics.md)). A variant in itself is not "pathogenic", whether it can be causally related to a phenotype observed in a patient is determined by other factors.
