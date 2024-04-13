# LatticeLSTM
It is the implemation of the paper [Chinese NER Using Lattice LSTM](https://arxiv.org/pdf/1805.02023.pdf) with pyTorch 1.8.1.

## Environment
+ python 3.8.1
+ pytorch==1.8.1

## Dataset
It is ResumeNER data, if you want to use your own dataset, the data need to be CoNLL format (prefer BIOES tag scheme), with each character its label for one line. Sentences are splited with a null line.

	美	B-LOC
	国	E-LOC
	的	O
	华	B-PER
	莱	I-PER
	士	E-PER

	我	O
	跟	O
	他	O
	谈	O
	笑	O
	风	O
	生	O 
  
  ## Quick Start:
1. Clone this code repository to your local machine:
```sh
$ git clone https://github.com/hualaobisi/LatticeLSTM.git
```
2. Install the required dependencies

3. Download the pretrained character and word embeddings and put them into the models directory(It is already done).

4. Run the training program:
```sh
$ bash run_train.sh
```
5. Run the predicting program:
```sh
$ bash run_predict.sh
```
