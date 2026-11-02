---
title: "PGE2 loop in the macrophage (Activity Flow, all molecules)"
topic: "PGE2 loop"
tab: "Activity Flow, all molecules"
page: ""
group: "Modelling"
order: 98
kind: "map"
draft: false
tag: "draft"
image: "/downloads/model-pge2-loop-af2.svg"
width: 1781
height: 1351
scale: 1
annotation: "/atlas-data/model-pge2-loop-af2.json"
image_error: ""
downloads:
  - {label: "GraphML", url: "/downloads/model-pge2-loop-af2.graphml"}
  - {label: "SVG", url: "/downloads/model-pge2-loop-af2.svg"}
---
The PGE2 loop as Activity Flow with every molecule of the Process Description map kept. Only the connections change. The inputs of a step meet in an AND gate, and two steps that make the same thing are alternatives. A molecule gets one node, and a second node only where one of its forms has a role of its own. So phosphorylated CREB is the activity of CREB, and protein kinase A is its catalytic subunit PRKACA held back by the regulatory subunit PRKAR1A until cyclic AMP binds it (Kim 2007). EP4 desensitisation is EP4 switching itself off after a delay (Nishigaki 1996).

## How removal is drawn

A remover that changes with the stimulus lowers what it removes. Phosphodiesterase 4B lowers cyclic AMP and is induced by lipopolysaccharide (Jin 2002, Jin 2005). A remover that is always there acts in its product instead. The prostaglandin transporter and 15-hydroxyprostaglandin dehydrogenase together make 15-keto-PGE2 from PGE2 outside the cell, the two-step route of PGE2 inactivation (Nomura 2004). PGE2 taken back up goes to oxidation and not out again (Nomura 2005), so uptake does not feed PGE2 in the cell. Where the product of a removal is not a node of its own, the activity stays on once made unless the remover is missing. CREB stays phosphorylated after protein kinase A stops only when protein phosphatase 1 is blocked, as phosphatase inhibitors prolong it (Hagiwara 1992).

## Why keep every molecule

Each molecule can now be switched off in the model. Blocking MRP4 (ABCC4, Reid 2003) keeps PGE2 inside the cell and leaves both receptors silent. Without the prostaglandin transporter no 15-keto-PGE2 is made. With protein phosphatase 1 gone, CREB keeps both genes on even after cyclic AMP has fallen and COX-2 is blocked. The behaviour without such changes is the same as in the other two tabs. While lipopolysaccharide is present, phosphodiesterase 4B keeps cyclic AMP down, and when the stimulus goes the loop either holds itself on through EP2 or switches off (Díaz-Muñoz 2012, Hinz 2000). In mouse macrophages lacking PDE4B the overall level of cyclic AMP did not change (Jin 2005), so this brake may act on a local pool of cyclic AMP, not on the whole cell.

The arc from RELA to the PTGS2 gate is green because it is disputed. The NF-κB site of the PTGS2 promoter was not needed for induction by endotoxin in RAW 264.7 cells (Wadleigh 2000), while other work found the promoter elements redundant (Mestre 2001).

## Source

New content, a third view of the module in the Process Description tab, with the same statements and references.

## References

1. Díaz-Muñoz MD, Osma-García IC, Cacheiro-Llaguno C, Fresno M, Iñiguez MA. Coordinated up-regulation of cyclooxygenase-2 and microsomal prostaglandin E synthase 1 transcription by nuclear factor kappa B and early growth response-1 in macrophages. Cell Signal. 2010;22(10):1427-36. PMID: [20546888](https://pubmed.ncbi.nlm.nih.gov/20546888/){:target="_blank" rel="noopener"}. doi: [10.1016/j.cellsig.2010.05.011](https://doi.org/10.1016/j.cellsig.2010.05.011){:target="_blank" rel="noopener"}
1. Díaz-Muñoz MD, Osma-García IC, Fresno M, Iñiguez MA. Involvement of PGE2 and the cAMP signalling pathway in the up-regulation of COX-2 and mPGES-1 expression in LPS-activated macrophages. Biochem J. 2012;443(2):451-61. PMID: [22268508](https://pubmed.ncbi.nlm.nih.gov/22268508/){:target="_blank" rel="noopener"}. doi: [10.1042/BJ20111052](https://doi.org/10.1042/BJ20111052){:target="_blank" rel="noopener"}
1. Gonzalez GA, Montminy MR. Cyclic AMP stimulates somatostatin gene transcription by phosphorylation of CREB at serine 133. Cell. 1989;59(4):675-80. PMID: [2573431](https://pubmed.ncbi.nlm.nih.gov/2573431/){:target="_blank" rel="noopener"}. doi: [10.1016/0092-8674(89)90013-5](https://doi.org/10.1016/0092-8674(89)90013-5){:target="_blank" rel="noopener"}
1. Hagiwara M, Alberts A, Brindle P, Meinkoth J, Feramisco J, Deng T, et al. Transcriptional attenuation following cAMP induction requires PP-1-mediated dephosphorylation of CREB. Cell. 1992;70(1):105-13. PMID: [1352481](https://pubmed.ncbi.nlm.nih.gov/1352481/){:target="_blank" rel="noopener"}. doi: [10.1016/0092-8674(92)90537-m](https://doi.org/10.1016/0092-8674(92)90537-m){:target="_blank" rel="noopener"}
1. Hinz B, Brune K, Pahl A. Prostaglandin E(2) upregulates cyclooxygenase-2 expression in lipopolysaccharide-stimulated RAW 264.7 macrophages. Biochem Biophys Res Commun. 2000;272(3):744-8. PMID: [10860826](https://pubmed.ncbi.nlm.nih.gov/10860826/){:target="_blank" rel="noopener"}. doi: [10.1006/bbrc.2000.2859](https://doi.org/10.1006/bbrc.2000.2859){:target="_blank" rel="noopener"}
1. Jin SL, Conti M. Induction of the cyclic nucleotide phosphodiesterase PDE4B is essential for LPS-activated TNF-alpha responses. Proc Natl Acad Sci U S A. 2002;99(11):7628-33. PMID: [12032334](https://pubmed.ncbi.nlm.nih.gov/12032334/){:target="_blank" rel="noopener"}. doi: [10.1073/pnas.122041599](https://doi.org/10.1073/pnas.122041599){:target="_blank" rel="noopener"}
1. Jin SL, Lan L, Zoudilova M, Conti M. Specific role of phosphodiesterase 4B in lipopolysaccharide-induced signaling in mouse macrophages. J Immunol. 2005;175(3):1523-31. PMID: [16034090](https://pubmed.ncbi.nlm.nih.gov/16034090/){:target="_blank" rel="noopener"}. doi: [10.4049/jimmunol.175.3.1523](https://doi.org/10.4049/jimmunol.175.3.1523){:target="_blank" rel="noopener"}
1. Kim C, Cheng CY, Saldanha SA, Taylor SS. PKA-I holoenzyme structure reveals a mechanism for cAMP-dependent activation. Cell. 2007;130(6):1032-43. PMID: [17889648](https://pubmed.ncbi.nlm.nih.gov/17889648/){:target="_blank" rel="noopener"}. doi: [10.1016/j.cell.2007.07.018](https://doi.org/10.1016/j.cell.2007.07.018){:target="_blank" rel="noopener"}
1. Mestre JR, Mackrell PJ, Rivadeneira DE, Stapleton PP, Tanabe T, Daly JM. Redundancy in the signaling pathways and promoter elements regulating cyclooxygenase-2 gene expression in endotoxin-treated macrophage/monocytic cells. J Biol Chem. 2001;276(6):3977-82. PMID: [11092878](https://pubmed.ncbi.nlm.nih.gov/11092878/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M005077200](https://doi.org/10.1074/jbc.M005077200){:target="_blank" rel="noopener"}
1. Neuschäfer-Rube F, Oppermann M, Möller U, Böer U, Püschel GP. Agonist-induced phosphorylation by G protein-coupled receptor kinases of the EP4 receptor carboxyl-terminal domain in an EP3/EP4 prostaglandin E(2) receptor hybrid. Mol Pharmacol. 1999;56(2):419-28. PMID: [10419563](https://pubmed.ncbi.nlm.nih.gov/10419563/){:target="_blank" rel="noopener"}. doi: [10.1124/mol.56.2.419](https://doi.org/10.1124/mol.56.2.419){:target="_blank" rel="noopener"}
1. Nishigaki N, Negishi M, Ichikawa A. Two Gs-coupled prostaglandin E receptor subtypes, EP2 and EP4, differ in desensitization and sensitivity to the metabolic inactivation of the agonist. Mol Pharmacol. 1996;50(4):1031-7. PMID: [8863851](https://pubmed.ncbi.nlm.nih.gov/8863851/){:target="_blank" rel="noopener"}.
1. Nomura T et al. The two-step model of prostaglandin signal termination: in vitro reconstitution with the prostaglandin transporter and prostaglandin 15 dehydrogenase. Mol Pharmacol. 2004. PMID: [15044627](https://pubmed.ncbi.nlm.nih.gov/15044627/){:target="_blank" rel="noopener"}. doi: [10.1124/mol.65.4.973](https://doi.org/10.1124/mol.65.4.973){:target="_blank" rel="noopener"}
1. Nomura T, Chang HY, Lu R, Hankin J, Murphy RC, Schuster VL. Prostaglandin signaling in the renal collecting duct: release, reuptake, and oxidation in the same cell. J Biol Chem. 2005;280(31):28424-9. PMID: [15855165](https://pubmed.ncbi.nlm.nih.gov/15855165/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M408286200](https://doi.org/10.1074/jbc.M408286200){:target="_blank" rel="noopener"}
1. Reid G, Wielinga P, Zelcer N, van der Heijden I, Kuil A, de Haas M, Wijnholds J, Borst P. The human multidrug resistance protein MRP4 functions as a prostaglandin efflux transporter and is inhibited by nonsteroidal antiinflammatory drugs. Proc Natl Acad Sci U S A. 2003 Aug 5;100(16):9244-9. doi: 10.1073/pnas.1033060100. PMID: 12835412.
1. Wadleigh DJ, Reddy ST, Kopp E, Ghosh S, Herschman HR. Transcriptional activation of the cyclooxygenase-2 gene in endotoxin-treated RAW 264.7 macrophages. J Biol Chem. 2000;275(9):6259-66. PMID: [10692422](https://pubmed.ncbi.nlm.nih.gov/10692422/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.275.9.6259](https://doi.org/10.1074/jbc.275.9.6259){:target="_blank" rel="noopener"}
