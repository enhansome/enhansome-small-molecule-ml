# Awesome Small Molecule Machine Learning with stars

A curated list of awesome papers, data sets, frameworks, packages, blogs, and other resources related to machine learning for small-molecule drug discovery. Please [contribute](CONTRIBUTING.md)!

## Contents

* [Papers](#papers)
  * [Survey papers and books](#papers-surveys)
  * [Representation, transfer, and few-shot learning](#papers-representation)
  * [Generative algorithms](#papers-generative-algorithms)
  * [Hit finding and potency prediciton](#papers-hit-finding)
  * [ADME and toxicity prediction](#papers-adme-tox)
  * [Synthetic accessability and retrosynthetic planning](#papers-synthetic-accessibility)
  * [DNA-encoded libraries (DELs)](#dels)
  * [Visualization and interpretability](#papers-viz)
  * [MS/MS prediction](#papers-msms)
* [Data sets](#data-sets)
* [Frameworks, Libraries, and Software Tools](#frameworks)
* [Blogs](#blogs)
* [Twitter](#twitter)
* [Related lists](#related-lists)

## Papers

<a id="papers-surveys"></a>

### Survey papers and books

* Walters and Barzilay, 2021. [Critical assessment of AI in drug discovery](https://doi.org/10.1080/17460441.2021.1915982).
* White, 2021. [Deep Learning for Molecules and Materials](https://dmol.pub/).
* Coley, 2020. [Defining and Exploring Chemical Spaces](https://dspace.mit.edu/handle/1721.1/131238).
* Chuang et al, 2020. [Learning Molecular Representations for Medicinal Chemistry](https://pubs.acs.org/doi/10.1021/acs.jmedchem.0c00385).
* Walters and Barzilay, 2020. [Applications of Deep Learning in Molecule Generation and Molecular Property Prediction](https://pubs.acs.org/doi/10.1021/acs.accounts.0c00699).
* Cai et al, 2020. [Transfer Learning for Drug Discovery](https://doi.org/10.1021/acs.jmedchem.9b02147).

<a id="papers-representation"></a>

### Representation, transfer learning, and few-shot learning

* Ying et al, 2021. [Do Transformers Really Perform Bad for Graph Representation? (Graphormer paper)](https://arxiv.org/abs/2106.05234). \[[Code](https://github.com/microsoft/Graphormer) ⭐ 2,473 | 🐛 101 | 🌐 Python | 📅 2026-06-12]
* Yang et al, 2019. [Analyzing Learned Molecular Representations for Property Prediction (Chemprop)](https://pubs.acs.org/doi/10.1021/acs.jcim.9b00237). \[[Code](https://github.com/chemprop/chemprop) ⭐ 2,439 | 🐛 14 | 🌐 Python | 📅 2026-08-21]
* Hu et al, 2019. [Strategies for Pre-training Graph Neural Networks](https://arxiv.org/abs/1905.12265). \[[Code](https://github.com/snap-stanford/pretrain-gnns) ⭐ 1,070 | 🐛 39 | 🌐 Python | 📅 2023-07-29]
* Satorras et al, 2021. [E(n) Equivariant Graph Neural Networks](https://arxiv.org/abs/2102.09844). \[[Code](https://github.com/vgsatorras/egnn) ⭐ 546 | 🐛 5 | 🌐 Python | 📅 2022-02-23]
* Ahmad et al, 2021. [ChemBERTa-2: Towards Chemical Foundation Models](https://cloud.ml.jku.at/s/dZ7CwqBkHX97C6S). \[[Code](https://github.com/seyonechithrananda/bert-loves-chemistry) ⭐ 501 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2024-10-27]
* Rong et al., 2020. [Self-Supervised Graph Transformer on Large-Scale Molecular Data (GROVER paper)](https://arxiv.org/abs/2007.02835). \[[Code](https://github.com/tencent-ailab/grover) ⭐ 394 | 🐛 19 | 🌐 Python | 📅 2026-02-25]
* Wang et al, 2022. [Molecular Contrastive Learning of Representations via Graph Neural Networks](https://arxiv.org/pdf/2102.10056.pdf). \[[Code](https://github.com/yuyangw/MolCLR) ⭐ 325 | 🐛 11 | 🌐 Python | 📅 2023-11-04]
* Maziarka et al, 2020. [Molecule Attention Transformer](https://arxiv.org/pdf/2002.08264.pdf). \[[Code](https://github.com/ardigen/MAT) ⭐ 254 | 🐛 10 | 🌐 Python | 📅 2020-04-01]
* Stanley et al, 2021. [FS-Mol: A Few-Shot Learning Dataset of Molecules](https://openreview.net/forum?id=701FtuyLlAd). \[[Code](https://github.com/microsoft/FS-Mol) ⭐ 177 | 🐛 11 | 🌐 Python | 📅 2023-02-03]
* Li and Fourches, 2020. [Inductive transfer learning for molecular activity prediction: Next-Gen QSAR Models with MolPMoFiT](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00430-x). \[[Code](https://github.com/XinhaoLi74/MolPMoFiT) ⭐ 45 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2022-08-28]
* Xue et al, 2021. [X-MOL: large-scale pre-training for molecular understanding and diverse molecular analysis](https://www.biorxiv.org/content/10.1101/2020.12.23.424259v2.full). \[[Code](https://github.com/bm2-lab/X-MOL) ⭐ 38 | 🐛 2 | 🌐 Python | 📅 2021-10-08]
* Nguyen et al., 2020. [Meta-Learning GNN Initializations for Low-Resource Molecular Property Prediction
  ](https://arxiv.org/pdf/2003.05996.pdf) \[[Code](https://github.com/GSK-AI/meta-learning-qsar) ⭐ 34 | 🐛 0 | 🌐 Python | 📅 2020-07-20]
* Krenn et al, 2022. [SELFIES and the future of molecular string representations](https://arxiv.org/abs/2204.00056).
* Townshend et al, 2021. [ATOM3D: Tasks On Molecules in Three Dimensions](https://arxiv.org/abs/2012.04035).
* Chuang and Keiser, 2020. [Attention-Based Learning on Molecular Ensembles](https://arxiv.org/abs/2011.12820).
* Feinberg et al, 2018. [PotentialNet for Molecular Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acscentsci.8b00507).
* Altae-Tran et al, 2017. [Low Data Drug Discovery with One-Shot Learning](https://pubs.acs.org/doi/abs/10.1021/acscentsci.6b00367).

<a id="papers-generative-algorithms"></a>

### Generative algorithms

* Zhou et al, 2019. [Optimization of Molecules via Deep Reinforcement Learning](https://doi.org/10.1038/s41598-019-47148-x). \[[Code (official version)](https://github.com/google-research/google-research/tree/master/mol_dqn) ⭐ 38,643 | 🐛 1,989 | 🌐 Jupyter Notebook | 📅 2026-08-27] \[[PyTorch implementation](https://github.com/aksub99/MolDQN-pytorch) ⭐ 84 | 🐛 7 | 🌐 Python | 📅 2023-03-24]
* Bengio et al, 2021. [Flow Network based Generative Models for Non-Iterative Diverse Candidate Generation](https://arxiv.org/abs/2106.04399). \[[Code](https://github.com/bengioe/gflownet) ⭐ 686 | 🐛 9 | 🌐 Python | 📅 2023-02-28]
* Jin et al, 2018. [Junction Tree Variational Autoencoder for Molecular Graph Generation](https://arxiv.org/abs/1802.04364). \[[Code](https://github.com/wengong-jin/icml18-jtnn) ⭐ 565 | 🐛 30 | 🌐 Python | 📅 2022-12-01]
* Brown, 2019. [GuacaMol: Benchmarking Models for de Novo Molecular Design](https://doi.org/10.1021/acs.jcim.8b00839). \[[Code](https://github.com/BenevolentAI/guacamol) ⭐ 531 | 🐛 13 | 🌐 Python | 📅 2024-02-11]
* Jin et al, 2020. [Hierarchical Generation of Molecular Graphs using Structural Motifs](https://arxiv.org/abs/2002.03230). \[[Code](https://github.com/wengong-jin/hgraph2graph) ⭐ 442 | 🐛 44 | 🌐 Python | 📅 2022-06-28]
* You et al, 2019. [Graph Convolutional Policy Network for Goal-Directed Molecular Graph Generation](https://arxiv.org/abs/1806.02473). \[[Code](https://github.com/bowenliu16/rl_graph_generation) ⭐ 359 | 🐛 10 | 🌐 Python | 📅 2022-10-12]
* Polishchuk, 2020. [CReM: chemically reasonable mutations framework for structure generation](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00431-w). \[[Code](https://github.com/DrrDom/crem) ⭐ 284 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2026-08-28]
* Imrie et al, 2020. [Deep Generative Models for 3D Linker Design](https://pubs.acs.org/doi/10.1021/acs.jcim.9b01120). \[[Code](https://github.com/oxpig/DeLinker) ⭐ 138 | 🐛 1 | 🌐 Python | 📅 2022-11-06]
* Gao et al, 2021. [Amortized Tree Generation for Bottom-up Synthesis Planning and Synthesizable Molecular Design](https://arxiv.org/abs/2110.06389). \[[Code](https://github.com/wenhao-gao/SynNet) ⭐ 99 | 🐛 2 | 🌐 Python | 📅 2022-12-19]
* Berenger and Tsuda, 2021. [Molecular generation by Fast Assembly of (Deep)SMILES fragments](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00566-4). \[[Code](https://github.com/UnixJunkie/FASMIFRA) ⭐ 57 | 🐛 5 | 🌐 OCaml | 📅 2024-10-31]
* Takeuchi et al, 2021. [R-group replacement database for medicinal chemistry](https://www.future-science.com/doi/10.2144/fsoa-2021-0062).
* Popova et al, 2019. [MolecularRNN: Generating realistic molecular graphs with optimized properties
  ](https://arxiv.org/abs/1905.13372).
* Merk et al, 2018. [De Novo Design of Bioactive Small Molecules by Artificial Intelligence](https://pubmed.ncbi.nlm.nih.gov/29319225/).

<a id="papers-hit-finding"></a>

### Hit finding and potency prediciton

* Stärk et al, 2022. [EquiBind: Geometric Deep Learning for Drug Binding Structure Prediction](https://arxiv.org/abs/2202.05146). \[[Code](https://github.com/HannesStark/EquiBind) ⭐ 546 | 🐛 8 | 🌐 Python | 📅 2025-02-19]
* Graff et al, 2021. [Accelerating high-throughput virtual screening through molecular pool-based active learning](https://pubs.rsc.org/en/content/articlelanding/2021/sc/d0sc06805e). \[[Code](https://github.com/coleygroup/molpal) ⭐ 213 | 🐛 11 | 🌐 Jupyter Notebook | 📅 2024-06-15]
* García-Ortegón et al, 2021. [DOCKSTRING: easy molecular docking yields better benchmarks for ligand design](https://arxiv.org/abs/2110.15486). \[[Code](https://github.com/dockstring/dockstring) ⭐ 189 | 🐛 8 | 🌐 Python | 📅 2026-05-24] \[[Data](https://figshare.com/s/95f2fed733dec170b998)]
* Gentile et al, 2020. [Deep Docking: A Deep Learning Platform for Augmentation of Structure Based Drug Discovery](https://pubs.acs.org/doi/10.1021/acscentsci.0c00229). \[[Code](https://github.com/jamesgleave/Deep-Docking-NonAutomated) ⭐ 56 | 🐛 7 | 🌐 Python | 📅 2022-11-24]
* Bender et al, 2021. [A practical guide to large-scale docking](https://www.nature.com/articles/s41596-021-00597-z).
* Cáceres et al, 2020. [Adding Stochastic Negative Examples into Machine Learning Improves Molecular Bioactivity Prediction](https://pubs.acs.org/doi/10.1021/acs.jcim.0c00565).
* Lin et al, 2019. [Ultra-large library docking for discovering new chemotypes](https://www.nature.com/articles/s41586-019-0917-9).

<a id="papers-adme-tox"></a>

### ADME and toxicity prediction

* Karim et al, 2021. [CardioTox net: a robust predictor for hERG channel blockade based on deep learning meta-feature ensembles](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00541-z). \[[Code](https://github.com/Abdulk084/CardioTox) ⭐ 22 | 🐛 3 | 🌐 Python | 📅 2025-01-05]
* Cai et al, 2019. [Deep Learning-Based Prediction of Drug-Induced Cardiotoxicity](https://pubs.acs.org/doi/10.1021/acs.jcim.8b00769). \[[Code](https://github.com/ChengF-Lab/deephERG) ⭐ 9 | 🐛 1 | 🌐 Python | 📅 2019-12-18]
* Fradkin et al, 2022. [A Graph Neural Network Approach to Molecule Carcinogenicity Prediction](https://www.biorxiv.org/content/10.1101/2021.11.10.468094v1.abstract).
* Siramshetty et al, 2021. [Validating ADME QSAR Models Using Marketed Drugs](https://journals.sagepub.com/doi/10.1177/24725552211017520).
* Göller et al, 2020. [Bayer’s in silico ADMET platform: a journey of machine learning over the past two decades](https://doi.org/10.1016/j.drudis.2020.07.001).
* Ryu et al, 2020. [DeepHIT: a deep learning framework for prediction of hERG-induced cardiotoxicity](https://doi.org/10.1093/bioinformatics/btaa075). \[[Code](https://bitbucket.org/krictai/deephit/src/master/)]
* Ogura et al, 2019. [Support Vector Machine model for hERG inhibitory activities based on the integrated hERG database using descriptor selection by NSGA-II](https://www.nature.com/articles/s41598-019-47536-3). \[[Data](https://drugdesign.riken.jp/hERGdb/)]
* Lombardo et al, 2018. [In Silico Absorption, Distribution, Metabolism, Excretion, and Pharmacokinetics (ADME-PK): Utility and Best Practices](https://pubs.acs.org/doi/10.1021/acs.jmedchem.7b00487).

<a id="papers-synthetic-accessibility"></a>

### Synthetic accessability and retrosynthetic planning

* Dai et al, 2019. [Retrosynthesis Prediction with Conditional Graph Logic Network](https://arxiv.org/abs/2001.01408). \[[Code](https://github.com/Hanjun-Dai/GLN) ⭐ 143 | 🐛 7 | 🌐 Python | 📅 2022-12-10]
* Coley et al, 2018. [SCScore: Synthetic Complexity Learned from a Reaction Corpus](https://pubs.acs.org/doi/10.1021/acs.jcim.7b00622). \[[Code](https://github.com/connorcoley/scscore) ⭐ 122 | 🐛 9 | 🌐 Roff | 📅 2021-01-20] \[[DeepChem implementation](https://github.com/deepchem/deepchem/blob/master/deepchem/models/scscore.py) ⭐ 6,967 | 🐛 1,167 | 🌐 Python | 📅 2026-08-20]
* Fortunato et al, 2020. [Data augmentation and pretraining for template-based retrosynthetic prediction in computer-aided synthesis planning](https://pubs.acs.org/doi/10.1021/acs.jcim.0c00403).
* Koch et al, 2020. [Reinforcement Learning for Bioretrosynthesis](https://pubs.acs.org/doi/10.1021/acssynbio.9b00447).
* Somnath et al, 2020. [Learning Graph Models for Retrosynthesis Prediction](https://arxiv.org/abs/2006.07038).

<a id="dels"></a>

### DNA-encoded libraries (DELs)

* Lim et al, 2022. [Machine Learning on DNA-Encoded Library Count Data Using an Uncertainty-Aware Probabilistic Loss Function](https://pubs.acs.org/doi/10.1021/acs.jcim.2c00041). \[[Code](https://github.com/coleygroup/del_qsar) ⭐ 33 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2022-06-08]
* McCloskey et al, 2020. [Machine Learning on DNA-Encoded Libraries: A New Paradigm for Hit Finding](https://pubs.acs.org/doi/10.1021/acs.jmedchem.0c00452).

<a id="papers-viz"></a>

### Visualization and interpretability

* Humer et al, 2021. [ChemInformatics Model Explorer (CIME): Exploratory analysis of chemical model explanations](https://chemrxiv.org/engage/chemrxiv/article-details/61a6579f568d33caaa4bff69). \[[Code](https://github.com/jku-vds-lab/cime) ⭐ 32 | 🐛 2 | 🌐 TypeScript | 📅 2023-01-12]
* Matveieva and Polishchuk, 2021. [Benchmarks for interpretation of QSAR models](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00519-x). \[[Code](https://github.com/ci-lab-cz/ibenchmark) ⭐ 14 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2022-08-12]
* Atsushi et al, 2019. [Integrating the Structure–Activity Relationship Matrix Method with Molecular Grid Maps and Activity Landscape Models for Medicinal Chemistry Applications](https://pubs.acs.org/doi/10.1021/acsomega.9b00595).
* Naveja and Medina-Franco, 2019. [Finding Constellations in Chemical Space Through Core Analysis](https://www.frontiersin.org/articles/10.3389/fchem.2019.00510/full).

<a id="papers-msms"></a>

### MS/MS prediction

* Goldman el al, 2023. [Prefix-Tree Decoding for Predicting Mass Spectra from Molecules](https://arxiv.org/abs/2303.06470). \[[Code](https://github.com/samgoldman97/ms-pred) ⭐ 152 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2026-08-19]
* Wei et al, 2019. [Rapid Prediction of Electron–Ionization Mass Spectrometry Using Neural Networks](https://pubs.acs.org/doi/10.1021/acscentsci.9b00085). \[[Code](https://github.com/brain-research/deep-molecular-massspec) ⚠️ Archived]
* Young et al, 2023. [MassFormer: Tandem Mass Spectrum Prediction for Small Molecules using Graph Transformers](https://arxiv.org/abs/2111.04824). \[[Code](https://github.com/Roestlab/massformer) ⭐ 100 | 🐛 2 | 🌐 Python | 📅 2024-08-26]
* Hong et al, 2023. [3DMolMS: prediction of tandem mass spectra from 3D molecular conformations](https://academic.oup.com/bioinformatics/article/39/6/btad354/7186501). \[[Code](https://github.com/JosieHong/3DMolMS) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-08-12]
* Wang et al, 2021. [CFM-ID 4.0: More Accurate ESI-MS/MS Spectral Prediction and Compound Identification](https://pubs.acs.org/doi/10.1021/acs.analchem.1c01465).

## Data sets

* [ADME@NCATS](https://opendata.ncats.nih.gov/adme)
* [AMED Cardiotoxicity Database](https://drugdesign.riken.jp/hERGdb/)
* [BindingDB](https://www.bindingdb.org/bind/index.jsp)
* [ChEMBL](https://www.ebi.ac.uk/chembl/)
* [DrugBank](https://go.drugbank.com)
* [DrugMatrix](https://ntp.niehs.nih.gov/data/drugmatrix/)
* [Enamine Real database](https://enamine.net/compound-collections/real-compounds/real-database)
* [hERG Central](https://www.cambridgemedchemconsulting.com/news/index_files/81f15972727e1fe70ae7f37514bdab58-362.html)
* [MoleculeNet](https://moleculenet.org/)
* [MONA: DB of Mass spec + other readouts](https://mona.fiehnlab.ucdavis.edu/)
* [NPASS database of natural products](http://bidd.group/NPASS/)
* [PubChem](https://pubchem.ncbi.nlm.nih.gov/)
* [The Open Reaction Database](https://docs.open-reaction-database.org/en/latest/)
* [Therapeutic Data Commons](https://tdcommons.ai/)
* [Zinc](https://pubs.acs.org/doi/10.1021/acs.jcim.0c00675)

<a id="frameworks"></a>

## Frameworks, Libraries, and Software Tools

* [DeepChem](https://deepchem.io/) \[[Tutorials](https://github.com/deepchem/deepchem/tree/master/examples/tutorials) ⭐ 6,967 | 🐛 1,167 | 🌐 Python | 📅 2026-08-20]
* [Chemprop](https://github.com/chemprop/chemprop) ⭐ 2,439 | 🐛 14 | 🌐 Python | 📅 2026-08-21
* [rd\_filters](https://github.com/PatWalters/rd_filters) ⭐ 172 | 🐛 6 | 🌐 Python | 📅 2026-02-17
* [AutoDock Vina](https://autodock-vina.readthedocs.io/en/latest/index.html)
* [BioPandas](http://rasbt.github.io/biopandas/)
* [Open Babel](http://openbabel.org/wiki/Main_Page)
* [pdb-tools](http://www.bonvinlab.org/pdb-tools/)
* [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/)
* [Small-World Search](https://sw.docking.org/search.html)
* [TorchDrug](https://torchdrug.ai/)

## Blogs

* [Hyperparameter Space](http://hyperparameter.space/)
* [Is Life Worth Living](https://iwatobipen.wordpress.com/)
* [Practical Cheminformatics](http://practicalcheminformatics.blogspot.com/)
* [RDKit Blog](https://greglandrum.github.io/rdkit-blog/)

## Twitter

* [Regina Barzilay](https://twitter.com/BarzilayRegina)
* [Bob the Grumpy Med Chemist](https://twitter.com/med_chemist)
* [John Chodera](https://twitter.com/jchodera)
* [Connor W. Coley](https://twitter.com/cwcoley)
* [Greg Landrum](https://twitter.com/dr_greg_landrum)
* [pen(Taka)](https://twitter.com/iwatobipen)
* [Bharath Ramsundar](https://twitter.com/rbhar90)
* [Marwin Segler](https://twitter.com/marwinsegler)
* [Patrick Walters](https://twitter.com/wpwalters)

## Related lists

* [deeplearning-biology](https://github.com/hussius/deeplearning-biology#chemoinformatics-and-drug-discovery-) ⭐ 2,155 | 🐛 0 | 📅 2026-08-03
* [Awesome Explainable Graph Reasoning](https://github.com/AstraZeneca/awesome-explainable-graph-reasoning) ⭐ 1,990 | 🐛 0 | 📅 2022-04-04
* [Awesome Python Chemistry](https://github.com/lmmentel/awesome-python-chemistry) ⭐ 1,434 | 🐛 10 | 📅 2025-09-21
* [Awesome Cheminformatics](https://github.com/hsiaoyi0504/awesome-cheminformatics) ⭐ 880 | 🐛 35 | 📅 2024-03-15
* [Awesome Drug Discovery](https://github.com/xnuohz/awesome-drug-discovery) ⭐ 43 | 🐛 2 | 📅 2021-11-15

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
