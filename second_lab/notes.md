Results

### 10 200 300 ###
Recieved this error on:
16 GB MAC
32 GB Windows
64 GB AWS
numpy.core._exceptions._arraymemoryerror: unable to allocate 2.42 gib for an array with shape (8277, 131, 300) and data type float64

Fixed it by increase the virtual memory size of windows to 150GB


### XSS ###
Now predicting on train set (0.2 dropout)
1208/1208 ━━━━━━━━━━━━━━━━━━━━ 4s 3ms/step    
Accuracy: 0.9121294498381877
Precision: 0.9560647249190939
Recall: 0.5
F1 score: 0.477023


Now predicting on test set (0.2 dropout)
259/259 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step 
Accuracy: 0.9131327775764165
Precision: 0.9565663887882083
Recall: 0.5
F1 score: 0.477297


Now predicting on finaltest set (0.2 dropout)
259/259 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.9113205267609037
Precision: 0.9556602633804518
Recall: 0.5
F1 score: 0.476802

### path_disclosure ###
Now predicting on train set (0.2 dropout)
2871/2871 ━━━━━━━━━━━━━━━━━━━━ 11s 4ms/step    
Accuracy: 0.8839746521199451
Precision: 0.9419873260599725
Recall: 0.5
F1 score: 0.469207


Now predicting on test set (0.2 dropout)
616/616 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.8827803465271074
Precision: 0.9413901732635537
Recall: 0.5
F1 score: 0.468871


Now predicting on finaltest set (0.2 dropout)
615/615 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.8825711382113821
Precision: 0.9412855691056911
Recall: 0.5
F1 score: 0.468812


### remote_code_execution ###
ow predicting on train set (0.2 dropout)
2102/2102 ━━━━━━━━━━━━━━━━━━━━ 5s 2ms/step   
Accuracy: 0.9104899263995242
Precision: 0.9552449631997622
Recall: 0.5
F1 score: 0.476574


Now predicting on test set (0.2 dropout)
451/451 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.9127055721323989
Precision: 0.9563527860661994
Recall: 0.5
F1 score: 0.477180


Now predicting on finaltest set (0.2 dropout)
451/451 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.90917291146267
Precision: 0.954586455731335
Recall: 0.5
F1 score: 0.476213

### command_injection ###
Now predicting on train set (0.2 dropout)
2102/2102 ━━━━━━━━━━━━━━━━━━━━ 5s 2ms/step   
Accuracy: 0.9104899263995242
Precision: 0.9552449631997622
Recall: 0.5
F1 score: 0.476574


Now predicting on test set (0.2 dropout)
451/451 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.9127055721323989
Precision: 0.9563527860661994
Recall: 0.5
F1 score: 0.477180


Now predicting on finaltest set (0.2 dropout)
451/451 ━━━━━━━━━━━━━━━━━━━━ 1s 2ms/step  
Accuracy: 0.90917291146267
Precision: 0.954586455731335
Recall: 0.5
F1 score: 0.476213





<!-- Issue Notes -->

scrappingGithub.py
pip install requests
pip install requests_oauthlib
create all_commits.json
add exceptions for the requests 

gitDiff.json
import os
pip install keras
missing spell of datata to data




getData
ModuleNotFoundError: No module named 'keras.layers.convolutional'
from tensorflow.keras.layers import Conv1D
from tensorflow.keras.layers import MaxPooling1D
from keras.layers import Embedding

AttributeError: The vocab attribute was removed from KeyedVector in Gensim 4.0.0.
Use KeyedVector's .key_to_index dict, .index_to_key list, and methods .get_vecattr(key, attr) and .set_vecattr(key, attr, new_val) instead.
See https://github.com/RaRe-Technologies/gensim/wiki/Migrating-from-Gensim-3.x-to-4



File "/Applications/XAMPP/xamppfiles/htdocs/uni/insider-security/main/Code/makemodel.py", line 173, in <module>
    vector = w2v_model[t]
             ~~~~~~~~~^^^
TypeError: 'Word2Vec' object is not subscriptable


if t in word_vectors.vocab and t != " ":
      vector = w2v_model[t]

to

        if t in word_vectors.key_to_index and t != " ":
            vector = w2v_model.wv[t] 


            



