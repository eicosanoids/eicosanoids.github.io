---
title: "PGE2: more COX-2, less 5-LOX"
topic: "PGE2 feedback through cAMP"
tab: ""
page: ""
group: "Feedback"
order: 85
kind: "map"
draft: false
tag: "new"
image: "/downloads/feedback-pge2-camp.svg"
width: 1060
height: 1610
scale: 1
annotation: "/atlas-data/feedback-pge2-camp.json"
image_error: ""
downloads:
  - {label: "GraphML", url: "/downloads/feedback-pge2-camp.graphml"}
  - {label: "SVG", url: "/downloads/feedback-pge2-camp.svg"}
---
PGE2 changes how much eicosanoid a cell makes through its own receptor. Through EP2 it raises cyclic AMP, which frees the catalytic subunit of protein kinase A. The kinase phosphorylates CREB, and CREB with the PTGS2 gene drives the expression of cyclooxygenase-2, the enzyme that made the PGH2 in the first place. In renal medullary cells and in human amnion fibroblasts this is a positive loop: more PGE2 gives more COX-2, which gives more PGE2 (Steinert 2009, Lu 2019).

The same kinase phosphorylates 5-lipoxygenase on serine 523. The mark lowers the activity of the enzyme and keeps it out of the nucleus, where it would meet FLAP (Luo 2004, Luo 2005). So the loop that feeds the prostaglandin branch brakes the leukotriene branch, which draws on the same arachidonic acid.

How PGE2 reaches the PTGS2 gene depends on the cell. In colon cancer cells EP4 does it through Gi and the EGF receptor (Yoshida 2013), and in amnion fibroblasts EP4 damps the induction that EP2 starts (Lu 2019). Serine 523 of 5-lipoxygenase is phosphorylated in B cells after PGE2 but could not be found phosphorylated in human granulocytes and monocytes (Mahshid 2015), the cells in which this brake is usually assumed to work.

## Source

New content, marked "new" on the atlas list until reviewed. A loop map joins steps that the production, receptor and regulation maps draw one by one. The G protein cycle between a receptor and its second messenger is drawn in the receptor maps, so here the ligand:receptor complex stimulates the step it leads to. Gene expression is drawn as on the other maps of the atlas, without the nucleus.

## References

1. Hla T et al. 1992. Human cyclooxygenase-2 cDNA. Proc Natl Acad Sci U S A. [PMID:1380156](https://pubmed.ncbi.nlm.nih.gov/1380156/){:target="_blank" rel="noopener"}
1. Jakobsson PJ, Thorén S, Morgenstern R, Samuelsson B. Identification of human prostaglandin E synthase: a microsomal, glutathione-dependent, inducible enzyme, constituting a potential novel drug target. Proc Natl Acad Sci U S A. 1999 Jun 22;96(13):7220-5. doi: 10.1073/pnas.96.13.7220. PMID: 10377395.
1. Lu JW, Wang WS, Zhou Q, Gan XW, Myatt L, Sun K. Activation of prostaglandin EP4 receptor attenuates the induction of cyclooxygenase-2 expression by EP2 receptor activation in human amnion fibroblasts: implications for parturition. FASEB J. 2019;33(7):8148-8160. PMID: [30917001](https://pubmed.ncbi.nlm.nih.gov/30917001/){:target="_blank" rel="noopener"}. doi: [10.1096/fj.201802642R](https://doi.org/10.1096/fj.201802642R){:target="_blank" rel="noopener"}
1. Luo M, Jones SM, Flamand N, Aronoff DM, Peters-Golden M, Brock TG. Phosphorylation by protein kinase A inhibits nuclear import of 5-lipoxygenase. J Biol Chem. 2005;280(49):40609-16. PMID: [16230355](https://pubmed.ncbi.nlm.nih.gov/16230355/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M507045200](https://doi.org/10.1074/jbc.M507045200){:target="_blank" rel="noopener"}
1. Luo M, Jones SM, Phare SM, Coffey MJ, Peters-Golden M, Brock TG. Protein kinase A inhibits leukotriene synthesis by phosphorylation of 5-lipoxygenase on serine 523. J Biol Chem. 2004;279(40):41512-20. PMID: [15280375](https://pubmed.ncbi.nlm.nih.gov/15280375/){:target="_blank" rel="noopener"}. doi: [10.1074/jbc.M312568200](https://doi.org/10.1074/jbc.M312568200){:target="_blank" rel="noopener"}
1. Mahshid Y, Markoutsa S, Dincbas-Renqvist V, Sürün D, Christensson B, Sander B, et al. Phosphorylation of serine 523 on 5-lipoxygenase in human B lymphocytes. Prostaglandins Leukot Essent Fatty Acids. 2015;100:33-40. PMID: [26210919](https://pubmed.ncbi.nlm.nih.gov/26210919/){:target="_blank" rel="noopener"}. doi: [10.1016/j.plefa.2015.06.003](https://doi.org/10.1016/j.plefa.2015.06.003){:target="_blank" rel="noopener"}
1. Qu C et al. 2021. Ligand recognition, unconventional activation, and G protein coupling of the prostaglandin E(2) receptor EP2 subtype. Sci Adv. [PMID:33811074](https://pubmed.ncbi.nlm.nih.gov/33811074/){:target="_blank" rel="noopener"}
1. Regan JW, Bailey TJ, Pepperl DJ, Pierce KL, Bogardus AM, Donello JE, Fairbairn CE, Kedzie KM, Woodward DF, Gil DW. Cloning of a novel human prostaglandin receptor with characteristics of the pharmacologically defined EP2 subtype. Mol Pharmacol. 1994 Aug;46(2):213-20. PMID: 8078484.
1. Steinert D, Küper C, Bartels H, Beck FX, Neuhofer W. PGE2 potentiates tonicity-induced COX-2 expression in renal medullary cells in a positive feedback loop involving EP2-cAMP-PKA signaling. Am J Physiol Cell Physiol. 2009;296(1):C75-87. PMID: [19005164](https://pubmed.ncbi.nlm.nih.gov/19005164/){:target="_blank" rel="noopener"}. doi: [10.1152/ajpcell.00024.2008](https://doi.org/10.1152/ajpcell.00024.2008){:target="_blank" rel="noopener"}
1. Yoshida K, Fujino H, Otake S, Seira N, Regan JW, Murayama T. Induction of cyclooxygenase-2 expression by prostaglandin E2 stimulation of the prostanoid EP4 receptor via coupling to Gαi and transactivation of the epidermal growth factor receptor in HCA-7 human colon cancer cells. Eur J Pharmacol. 2013;718(1-3):408-17. PMID: [23973650](https://pubmed.ncbi.nlm.nih.gov/23973650/){:target="_blank" rel="noopener"}. doi: [10.1016/j.ejphar.2013.08.002](https://doi.org/10.1016/j.ejphar.2013.08.002){:target="_blank" rel="noopener"}
