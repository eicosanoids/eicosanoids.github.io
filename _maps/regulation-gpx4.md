---
title: "GPX4 and the aldehyde it prevents"
topic: "Regulation of GPX4"
tab: ""
page: ""
group: "Regulation"
order: 79
kind: "map"
draft: false
tag: "new"
image: "/downloads/regulation-gpx4.svg"
width: 869
height: 730
scale: 1
annotation: "/atlas-data/regulation-gpx4.json"
image_error: ""
downloads:
  - {label: "GraphML", url: "/downloads/regulation-gpx4.graphml"}
  - {label: "SVG", url: "/downloads/regulation-gpx4.svg"}
---
GPX4 reduces the hydroperoxides in membrane lipids, which is what keeps a cell from ferroptosis, and the lipoxygenase products of this atlas are among its substrates. The regulation drawn here is a loop that closes on itself. 4-hydroxynonenal, an aldehyde that comes from the same lipid peroxidation GPX4 prevents, carbonylates cysteine 93 of the enzyme. That adduct keeps the deubiquitinase OTUD5 from binding, so the ubiquitin chain that would have been removed stays on and the enzyme is destroyed. The same aldehyde also carbonylates OTUD5 itself, on cysteine 247, and raising OTUD5 stabilises GPX4 again (Zhang 2023).

The mitochondrial pool of the enzyme is also held by acetylation, which SIRT3 removes. Without SIRT3 the acetylation rises, GPX4 falls and cells go to ferroptosis (Wang 2024). That part is not drawn, as the evidence is from mouse kidney.

The work on the ubiquitin loop is from cardiomyocytes and the mouse heart.

## Source

New content, marked "new" on the atlas list until reviewed. Every step carries its references, each checked against its PubMed record. The marks on the enzymes are drawn as state variables, and a mark that SBGN does not name (HNE for the aldehyde adduct, NO2 for nitration, G for the sugar, LTA4 for the covalent adduct of the substrate) is explained in this text.

## References

1. Guo YY, Liang NN, Zhang XY, Ren YH, Wu WZ, Liu ZB, et al. Mitochondrial GPX4 acetylation is involved in cadmium-induced renal cell ferroptosis. Redox Biol. 2024;73:103179. PMID: [38733909](https://pubmed.ncbi.nlm.nih.gov/38733909/){:target="_blank" rel="noopener"}. doi: [10.1016/j.redox.2024.103179](https://doi.org/10.1016/j.redox.2024.103179){:target="_blank" rel="noopener"}
1. Imai H, Narashima K, Arai M, Sakamoto H, Chiba N, Nakagawa Y. Suppression of leukotriene formation in RBL-2H3 cells that overexpressed phospholipid hydroperoxide glutathione peroxidase. J Biol Chem. 1998;273(4):1990-7. PMID: [9442035](https://pubmed.ncbi.nlm.nih.gov/9442035/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.273.4.1990](https://doi.org/10.1074/jbc.273.4.1990){:target="_blank" rel="noopener"}
1. Liu L, Pang J, Qin D, Li R, Zou D, Chi K, et al. Deubiquitinase OTUD5 as a Novel Protector against 4-HNE-Triggered Ferroptosis in Myocardial Ischemia/Reperfusion Injury. Adv Sci (Weinh). 2023;10(28):e2301852. PMID: [37552043](https://pubmed.ncbi.nlm.nih.gov/37552043/){:target="_blank" rel="noopener"}. doi: [10.1002/advs.202301852](https://doi.org/10.1002/advs.202301852){:target="_blank" rel="noopener"}
1. Sutherland M, Shankaranarayanan P, Schewe T, Nigam S. Evidence for the presence of phospholipid hydroperoxide glutathione peroxidase in human platelets: implications for its involvement in the regulatory network of the 12-lipoxygenase pathway of arachidonic acid metabolism. Biochem J. 2001;353(Pt 1):91-100. PMID: [11115402](https://pubmed.ncbi.nlm.nih.gov/11115402/){:target="_blank" rel="noopener"}.
