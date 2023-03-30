# Disclaimer

This is a research project and by definition is unstable. Please write to us if you find something not correct or strange. We are sharing the codes under the condition that reproducing full or part of codes must cite the related papers.

# Related Papers
- Zhou Q, Li R, Zhao Z, et al. Adaptive Bit Rate Control in Semantic Communication with Incremental Knowledge-based HARQ[J]. arXiv preprint arXiv:2203.06634, 2022, accepted by IEEE Open Journal of the Communications Society. https://arxiv.org/pdf/2108.09119

- Zhou Q, Li R, Zhao Z, et al. Semantic communication with adaptive universal transformer[J]. IEEE Wireless Communications Letters, 2021, 11(3): 453-457,
accepted IEEE Wireless Communications Letters. https://arxiv.org/pdf/2203.06634

# Dataset:
For dataset, it is available online at http://www.statmt.org/europarl/

Choose the file "parallel corpus French-English, 194 MB, 04/1996-11/2011".

# Run the code:
To *pre-process the data*: preprocess_captions.py

- Note: The file "parallel corpus French-English, 194 MB, 04/1996-11/2011" shall be downloaded [online](http://www.statmt.org/europarl/). Then, the file "english.pkl" is expected to be obtained after using "preprocess_captions.py" to preprocess the file "fr-en.tgz".

To *get the baseline*: modeltrainbase.py

To *get the result after quantification*: modeltrainbasequantification1.py and modeltrainbasequantification2.py

Train with *Universal Transformer (UT)*: modeltrainUT.py 

Train with *Incremental Knowledge-HARQ (IK-HARQ)*: modeltrainIKHARQ.py

Train with *Denoiser*: modeltraindenoiser1.py and modeltraindenoiser2.py

Train with *Adaptive Bit Rate control*: modeltrainmultibitratepart(1/2/3).py, modeltrainpolicynetpart(1/2).py
