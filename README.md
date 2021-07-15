# DeepBinDiff_edited


Requirements:
```
    tensorflow (2.0 > tensorflow version >= 1.14.0)
    gensim
    angr
    networkx
    lapjv -> Needs downgrade
```

Edited
```
1. lapjv -> downgraded 1.3.0
2. pip3 install scipy==1.4.1
2. pip3 install -U scikit-learn matplotlib
3. mkdir data
4. mkdir data/DeepBD
6. src/deepwalk/skimgram.py in line'from gensim.models.word2vec import Vocab'removal
7. src/libnrl/gcn/layers.py in line 4  -> tensorflow.compat.v1 added
8. src/libnrl/gcn/gcnAPI.py -> tensorflow.compat.v1 added
9. src/deepbindiff.py -> tensorflow.compat.v1 added
