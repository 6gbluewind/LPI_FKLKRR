Identifying LncRNA-Protein Interaction with Kernel Ridge Regression based on Fast Kernel Learning
==== 
### About
We develop a novel prediction method of lncRNAs-protein interactions (LPIs) by using kernel ridge regression with multiple kernel learning approach. The output contains five files, named bench_auc.fig, bench_loo_pr, bench_loo_roc.fig, bench_pr.fig and result.mat. Generally, our method can handle prediction of LPIs in several seconds with high performance machine.

Input: Similarity of lncRNAs, including K_GIP, K_SW, K_SF, K_EXP;<br />
       Similarity of proteins, including K_GIP, K_SW, K_SF, K_GO<br />
Similarity matrices construction:<br />
       Gauss similarity matrix is constructed by the kernel_gip.m,<br />
       kernel_lncRNA_feature_CT, SW_lncRNA_Similarity, kernel_lncRNA_feature_expression,<br />
       kernel_protein_feature_PsePSSM, SW_Protein_Similarity, protein_GO_Jacard in input_info.mat are precalculated similarity matrices.<br />
Four kinds of kernels in lncRNA or protein space is fusing with fast kernel learning, which is achieved with fast_kernels_weight.m; KRR codes corresponds to tsKRR.m file. In practice, all the codes and results are packing in the form of .rar files to faciliate uploading or downloading. 
       
### Software
To run our program, put the input_info.mat and the code files under the same directory.
The 5-fold cross-validation demo is "sample2_ridge.m"
The leave one out cross-validation demo is "sample2_loo.m"
       
#### Environment
* MATLAB 
* 4-core CPU
* 20 GB memory
* 64-bit Windows Operating Systems

### Data
There are two datasets in the folder. 
* Benchmark dataset is illustrated in [3]. This dataset contains 4158 lncRNA-protein interactions, 990 lncRNAs and 27 proteins.
* Novel dataset is proposed in [4]. This novel dataset consists of 4467 LPIs, including 1050 unique lncRNAs and 84 unique proteins.

### Result
bench_auc.fig, bench_loo_pr, bench_loo_roc.fig, bench_pr.fig and result.mat are the outcomes. <br />
Also, we give the case study results in local_cases folder.

### References:

[1] J. He, S.F. Chang, and L. Xie, “Fast kernel learning for spatial pyramid matching,” in CVPR 2008, pp. 1–7, June 2008.

[2] M. Stock, T. Pahikkala, A. Airola, B. D. Baets, and W. Waegeman, “Efficient pairwise learning using kernel ridge regression: an exact two step method,” 2016. arXiv:1606.04275

[3] W. Zhang, Q. Qu, Y. Zhang, W. Wang, W. Zhang, Q. Qu, Y. Zhang, and W. Wang, “The linear neighborhood propagation method for predicting
long non-coding RNA-protein interactions,” Neurocomputing, vol. 273, pp. 526–534, 2017.

[4] X. Zheng, Y. Wang, K. Tian, J. Zhou, J. Guan, L. Luo, and S. Zhou, “Fusing multiple protein-protein similarity networks to effectively
predict lncRNA-protein interactions,” BMC Bioinformatics, vol. 18, no. Suppl 12, p. 420, 2017.

