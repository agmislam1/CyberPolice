# Detecting-Cyberbullying-Across-SMPs

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


### Reproducibility Study 

1. Maral Dadvar, and Kai Eckert. "[Cyberbullying Detection in Social Networks Using Deep Learning Based Models; A Reproducibility Study.](https://arxiv.org/pdf/1812.08046.pdf)" arXiv preprint arXiv:1812.08046 (2018).
2. Aymé Arango, Jorge Pérez, and Barbara Poblete. "[Hate Speech Detection is Not as Easy as You May Think: A Closer Look at Model Validation.](https://users.dcc.uchile.cl/~jperez/papers/sigir2019.pdf)" Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval. ACM, 2019. 
3. Chris Emmery, Ben Verhoeven, Guy De Pauw, Gilles Jacobs, Cynthia Van Hee, Els Lefever, Bart Desmet, Véronique Hoste, Walter Daelemans. "[Current Limitations in Cyberbullying Detection: On Evaluation Criteria, Reproducibility, and Data Scarcity."](http://arxiv.org/abs/1910.11922) ArXiv:1910.11922 [Cs], Oct. 2019. arXiv.org. [[Code]](https://github.com/cmry/amica)

In [2] and [3], the authors discuss the limitations of our oversampling method (Section 4.2) in that, the way oversampling is currently handled may lead to overfitting. We found their claims/criticisms valid and important but we haven't conducted any new experiments to explicitely test and improve upon the limitations. Based on these studies, we no longer claim that our models provide state of the art results on the dataset untill further experiments are carried to study the effect of oversampling on the representations learned. We do believe that our paper and repository still serves as a useful resourse for modelling cyberbullying detection and understanding transferability between platforms. We suggest our viewers to look at these papers to be more aware of the limitations. 
 
