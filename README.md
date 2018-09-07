# LPI_FKLKRR
Identifying LPI with Kernel Ridge Regression based on Fast Kernel Learning
Input: Similarity of lncRNAs, including K_GIP, K_SW, K_SF, K_EXP;
       Similarity of proteins, including K_GIP, K_SW, K_SF, K_GO
Similarity matrices construction:
       Gauss similarity matrix is constructed by the kernel_gip.m
      
The 5-fold cross-validation demo is "sample2_ridge.m"
The leave one out cross-validation demo is "sample2_loo.m"
