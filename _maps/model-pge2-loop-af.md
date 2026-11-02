---
title: "PGE2 loop in the macrophage (Activity Flow)"
topic: "PGE2 loop"
tab: "Activity Flow"
page: ""
group: "Modelling"
order: 97
kind: "map"
draft: false
tag: "draft"
image: "/downloads/model-pge2-loop-af.svg"
width: 1165
height: 1210
scale: 1
annotation: "/atlas-data/model-pge2-loop-af.json"
image_error: ""
downloads:
  - {label: "GraphML", url: "/downloads/model-pge2-loop-af.graphml"}
  - {label: "SVG", url: "/downloads/model-pge2-loop-af.svg"}
---
The PGE2 loop of the Process Description tab, drawn as Activity Flow: each node is the activity of a molecule, and each arc says that one activity raises or lowers another. This is the form a Boolean model takes, so the map can be read as the model itself. A node is on when any arc raising it is on and no arc lowering it is on. The AND gate needs both of its inputs. RELA (NF-κB) and PDE4B are the inputs and stand for lipopolysaccharide, which activates NF-κB and induces phosphodiesterase 4B in macrophages (Díaz-Muñoz 2010, Jin 2005).

## What changes from the Process Description

Steps that remove something become arcs that lower it. Phosphodiesterase 4B lowers cyclic AMP, and desensitised EP4 lowers active EP4 (Nishigaki 1996, Neuschäfer-Rube 1999). Phosphorylation and dephosphorylation of CREB become one node, CREB activity. The dephosphorylation by protein phosphatase 1 (Hagiwara 1992) has no arc because the phosphatase is always active, so CREB activity simply follows protein kinase A. The same holds for the transporters and 15-hydroxyprostaglandin dehydrogenase, which take PGE2 up and oxidise it all the time (Nomura 2004). Their clearance sets how fast PGE2 falls once synthesis stops, which a Boolean model cannot show. The steps of protein kinase A activation are one node.

## The rules

| Node | On when |
|---|---|
| PTGS2 mRNA, PTGES mRNA | CREB or RELA |
| PTGS2, PTGES | their mRNA |
| PGH2 | PTGS2 |
| PGE2 in the cell | PGH2 and PTGES |
| PGE2 outside | PGE2 in the cell |
| 15-keto-PGE2 | PGE2 outside |
| PTGER2 | PGE2 outside |
| PTGER4 | PGE2 outside and not desensitised PTGER4 |
| desensitised PTGER4 | PTGER4 |
| cAMP | PTGER2 or PTGER4, and not PDE4B |
| PRKACA | cAMP |
| CREB | PRKACA |

## What the model says

With lipopolysaccharide, NF-κB drives both genes and PGE2 is made, while phosphodiesterase 4B keeps cyclic AMP off. In mouse macrophages lacking PDE4B the overall level of cyclic AMP did not change (Jin 2005), so this brake may act on a local pool of cyclic AMP, not on the whole cell. When the stimulus goes, the loop either holds itself on through EP2 or switches off, depending on whether cyclic AMP reaches CREB before the messenger RNAs fall (Díaz-Muñoz 2012, Hinz 2000). This is the same result as the rules written for the Process Description map. One node behaves differently. Active and desensitised EP4 switch each other on and off in turn, because a Boolean negative loop of two nodes oscillates. In a cell EP4 stays desensitised while PGE2 is present.

The arc from RELA to PTGS2 mRNA is green because it is disputed. In RAW 264.7 cells the NF-κB site of the PTGS2 promoter was not needed for induction by endotoxin (Wadleigh 2000), while other work found the promoter elements redundant (Mestre 2001).

## Source

New content, a second view of the module in the Process Description tab, with the same statements and references.

## References

1. Díaz-Muñoz MD, Osma-García IC, Cacheiro-Llaguno C, Fresno M, Iñiguez MA. Coordinated up-regulation of cyclooxygenase-2 and microsomal prostaglandin E synthase 1 transcription by nuclear factor kappa B and early growth response-1 in macrophages. Cell Signal. 2010;22(10):1427-36. PMID: [20546888](https://pubmed.ncbi.nlm.nih.gov/20546888/){:target="_blank" rel="noopener"}. doi: [10.1016/j.cellsig.2010.05.011](https://doi.org/10.1016/j.cellsig.2010.05.011){:target="_blank" rel="noopener"}
1. Díaz-Muñoz MD, Osma-García IC, Fresno M, Iñiguez MA. Involvement of PGE2 and the cAMP signalling pathway in the up-regulation of COX-2 and mPGES-1 expression in LPS-activated macrophages. Biochem J. 2012;443(2):451-61. PMID: [22268508](https://pubmed.ncbi.nlm.nih.gov/22268508/){:target="_blank" rel="noopener"}. doi: [10.1042/BJ20111052](https://doi.org/10.1042/BJ20111052){:target="_blank" rel="noopener"}
1. Hagiwara M, Alberts A, Brindle P, Meinkoth J, Feramisco J, Deng T, et al. Transcriptional attenuation following cAMP induction requires PP-1-mediated dephosphorylation of CREB. Cell. 1992;70(1):105-13. PMID: [1352481](https://pubmed.ncbi.nlm.nih.gov/1352481/){:target="_blank" rel="noopener"}. doi: [10.1016/0092-8674(92)90537-m](https://doi.org/10.1016/0092-8674(92)90537-m){:target="_blank" rel="noopener"}
1. Hinz B, Brune K, Pahl A. Prostaglandin E(2) upregulates cyclooxygenase-2 expression in lipopolysaccharide-stimulated RAW 264.7 macrophages. Biochem Biophys Res Commun. 2000;272(3):744-8. PMID: [10860826](https://pubmed.ncbi.nlm.nih.gov/10860826/){:target="_blank" rel="noopener"}. doi: [10.1006/bbrc.2000.2859](https://doi.org/10.1006/bbrc.2000.2859){:target="_blank" rel="noopener"}
1. Jin SL, Lan L, Zoudilova M, Conti M. Specific role of phosphodiesterase 4B in lipopolysaccharide-induced signaling in mouse macrophages. J Immunol. 2005;175(3):1523-31. PMID: [16034090](https://pubmed.ncbi.nlm.nih.gov/16034090/){:target="_blank" rel="noopener"}. doi: [10.4049/jimmunol.175.3.1523](https://doi.org/10.4049/jimmunol.175.3.1523){:target="_blank" rel="noopener"}
1. Mestre JR, Mackrell PJ, Rivadeneira DE, Stapleton PP, Tanabe T, Daly JM. Redundancy in the signaling pathways and promoter elements regulating cyclooxygenase-2 gene expression in endotoxin-treated macrophage/monocytic cells. J Biol Chem. 2001;276(6):3977-82. PMID: [11092878](https://pubmed.ncbi.nlm.nih.gov/11092878/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M005077200](https://doi.org/10.1074/jbc.M005077200){:target="_blank" rel="noopener"}
1. Neuschäfer-Rube F, Oppermann M, Möller U, Böer U, Püschel GP. Agonist-induced phosphorylation by G protein-coupled receptor kinases of the EP4 receptor carboxyl-terminal domain in an EP3/EP4 prostaglandin E(2) receptor hybrid. Mol Pharmacol. 1999;56(2):419-28. PMID: [10419563](https://pubmed.ncbi.nlm.nih.gov/10419563/){:target="_blank" rel="noopener"}. doi: [10.1124/mol.56.2.419](https://doi.org/10.1124/mol.56.2.419){:target="_blank" rel="noopener"}
1. Nishigaki N, Negishi M, Ichikawa A. Two Gs-coupled prostaglandin E receptor subtypes, EP2 and EP4, differ in desensitization and sensitivity to the metabolic inactivation of the agonist. Mol Pharmacol. 1996;50(4):1031-7. PMID: [8863851](https://pubmed.ncbi.nlm.nih.gov/8863851/){:target="_blank" rel="noopener"}.
1. Nomura T et al. The two-step model of prostaglandin signal termination: in vitro reconstitution with the prostaglandin transporter and prostaglandin 15 dehydrogenase. Mol Pharmacol. 2004. PMID: [15044627](https://pubmed.ncbi.nlm.nih.gov/15044627/){:target="_blank" rel="noopener"}. doi: [10.1124/mol.65.4.973](https://doi.org/10.1124/mol.65.4.973){:target="_blank" rel="noopener"}
1. Nomura T, Chang HY, Lu R, Hankin J, Murphy RC, Schuster VL. Prostaglandin signaling in the renal collecting duct: release, reuptake, and oxidation in the same cell. J Biol Chem. 2005;280(31):28424-9. PMID: [15855165](https://pubmed.ncbi.nlm.nih.gov/15855165/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M408286200](https://doi.org/10.1074/jbc.M408286200){:target="_blank" rel="noopener"}
1. Wadleigh DJ, Reddy ST, Kopp E, Ghosh S, Herschman HR. Transcriptional activation of the cyclooxygenase-2 gene in endotoxin-treated RAW 264.7 macrophages. J Biol Chem. 2000;275(9):6259-66. PMID: [10692422](https://pubmed.ncbi.nlm.nih.gov/10692422/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.275.9.6259](https://doi.org/10.1074/jbc.275.9.6259){:target="_blank" rel="noopener"}
