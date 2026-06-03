# Optimizing MSM registration parameters fixes local minima issues on the dHCP database.

MSM [Multimodal Surface Matching](https://github.com/ecr05/MSM_HOCR/tree/master) is the state-of-the-art method for spherical registration of cortical surfaces obtained from MRI data. The alignment can be driven by various univariate,multivariate, or multimodal feature sets. This method is commonly used in the community for routine registrations and in particular for data released by the [Human Connectome Project](https://www.humanconnectome.org/).

However, when applied to neonatal dHCP data, the method may produce suboptimal registrations due to high variability in cortical folding and challenges in establishing accurate inter-subject correspondence.

We provide the configuration file for the method, which includes a rigid initialization step with high smoothing of source and target sulcal depth features to reduce local minima issues.

When using this work, please cite:

## References
Robinson, Emma C., Saad Jbabdi, Matthew F. Glasser, Jesper Andersson, Gregory C. Burgess, Michael P. Harms, Stephen M. Smith, David C. Van Essen, and Mark Jenkinson. "MSM: A new flexible framework for Multimodal Surface Matching." Neuroimage 100 (2014): 414-426.

Robinson, E.C., Garcia, K., Glasser, M.F., Chen, Z., Coalson, T.S., Makropoulos, A., Bozek, J., Wright, R., Schuh, A., Webster, M. and Hutter, J., 2017. Multimodal surface matching with higher-order smoothness constraints. NeuroImage.

Ishikawa, Hiroshi. "Higher-order clique reduction without auxiliary variables." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2014.

N. Komodakis and G. Tziritas "Approximate Labeling via Graph-Cuts Based on Linear Programming". IEEE Transactions on Pattern Analysis and Machine Intelligence, 2007.

Glocker, Ben, et al. "Triangleflow: Optical flow with triangulation-based higher-order likelihoods." European Conference on Computer Vision. Springer Berlin Heidelberg, 2010.
