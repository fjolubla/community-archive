
## Dataset overview

This Poseidon v3.0.0 package contains 71 ancient human genotype records from Fiji (49), Vanuatu (15), Tonga (4), and the Solomon Islands (3), associated with Feldman et al. (2026). The records have 70 distinct `Individual_ID` values because two genotype records, `SIG050` and `SIG053`, share the individual identifier `SIG050_053`.

The package uses binary PLINK genotype data (`2026_Feldman_Oceania.bed`, `.bim`, `.fam`), with the SNP set declared as `1240K` in `POSEIDON.yml`. Metadata are provided in `2026_Feldman_Oceania.janno`. The bibliography is `FeldmanCell2026.bib`; `FeldmanCell2026` is the publication key used in the Janno file.

## Chronological metadata

Dates were transcribed from Feldman et al. (2026), supplementary Tables S1A and S1B, with references to earlier studies where given. 

For `SIG050` and `SIG053` (burial 92b), the two radiocarbon determinations MAMS-49658 and MAMS-49661 are recorded together because the assignment of each determination to one of the two genotype records is unresolved. Their `Date_BC_AD_Start`, `Date_BC_AD_Median`, and `Date_BC_AD_Stop` values are left as `n/a` instead of choosing an unsupported single date. Details are noted in `Date_Note`.

## Individual identifiers and genetic relatedness

Relatedness assignments were compiled from Feldman et al. (2026), supplementary Table S1Q. Where library-level assignments for a pair conflicted, the closest reported relationship degree was used for reporting, in this order:

`first > second > thirdToFifth > unrelated`

This rule is a metadata reporting convention, not a claim that the selected degree is the statistically most likely relationship. Original library-level assignments should be consulted in supplementary Table S1Q.

## Sequencing source metadata

The sequencing source file (`2026_Feldman_Oceania.ssf`) contains 86 sequencing runs associated with the 71 genotype records. Sequencing accessions and associated metadata were obtained from ENA study PRJEB102472.

Library preparation types were compiled primarily from Feldman et al. (2026), supplementary Table S1C. Missing UDG treatment assignments were inferred from the laboratory preparation protocols described in the publication: double-stranded libraries were assigned `half` and single-stranded libraries were assigned `minus`. These inferred assignments are not independently verified library-specific UDG measurements.

The library preparation types of `SIG002.A0101.TF1.1`, `SIG014.A0101.TF1.1`, and `SIG050.A0101.TF1.1` remain unresolved because the available supplementary metadata do not unambiguously identify their library-specific preparation methods. Their `library_built` values were reported as `n/a`.

For `SIG052.A0101.TF1.1`, supplementary Table S1A reports `ssLibrary 2.0 2018`, whereas Table S1C identifies the specific library as `dsDNA`. The library type was retained as `ds` based on Table S1C, while its UDG treatment was set to `n/a` pending clarification.

The UDG treatments of `SIG002.A0101.TF1.1` and `SIG014.A0101.TF1.1` also remain unresolved. `SIG050.A0101.TF1.1` retains its pre-existing `udg = minus` assignment, although its original source has not yet been independently verified.
