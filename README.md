# DNN Models to Detect Cyberbullying

Abstract. As the number of people using social media increases rapidly, cyber bullying has become a severe problem. To express ideas, people are fre quently seen verbally attacking another. For many people, the impacts of cyberbullying remain longer. So, it is high time to detect such bul lies and hateful comments on social media and take appropriate action. To resolve this issue in this project, we want to make a model that can detect such comments automatically. We used four deep neural network models - Long Short-Term Memory(LSTM), stacked LSTM, Bidirectional LSTM with multi-head attention, and stacked Bidirectional LSTM with attention and compared which model gave the most accurate result. After training these models with the Twitter dataset, we found out that LSTM performed the worst among the four models, while stacked LSTM better classified sexism than other models. For classifying racism, bidirectional LSTM with multi-head attention gave the best F1-score among the other models.

## Dataset

We used twitter dataset which can be found in the data folder in pkl format.

### Prerequisites

The following commands need to run to create the environment

pip install pywin32

pip install tensorflow==1.15.2

* pip install sklearn
* pip install matplotlib
* pip install keras
* pip install pandas
* pip install textblob
* pip install git+https://github.com/tflearn/tflearn.git
* pip install tweet-preprocessor
* pip install numpy==1.19.5

### Instructions to run

 - models.py : All the model architectures are defined in this file.
 - DNNs.ipynb : This notebook is responsible for training DNN models (LSTM, stacked LSTM, bi-directional LSTM with multi-head attention, stacked bi-directional LSTM with attention ) to initialize random word embeddings.

Once the model is run, corresponding precision, recall & F1-score will be generated


### References 

1. Maral Dadvar, and Kai Eckert. "[Cyberbullying Detection in Social Networks Using Deep Learning Based Models; A Reproducibility Study.](https://arxiv.org/pdf/1812.08046.pdf)" arXiv preprint arXiv:1812.08046 (2018).
2. Aymé Arango, Jorge Pérez, and Barbara Poblete. "[Hate Speech Detection is Not as Easy as You May Think: A Closer Look at Model Validation.](https://users.dcc.uchile.cl/~jperez/papers/sigir2019.pdf)" Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval. ACM, 2019. 
3. Chris Emmery, Ben Verhoeven, Guy De Pauw, Gilles Jacobs, Cynthia Van Hee, Els Lefever, Bart Desmet, Véronique Hoste, Walter Daelemans. "[Current Limitations in Cyberbullying Detection: On Evaluation Criteria, Reproducibility, and Data Scarcity."](http://arxiv.org/abs/1910.11922) ArXiv:1910.11922 [Cs], Oct. 2019. arXiv.org. [[Code]](https://github.com/cmry/amica)


 
