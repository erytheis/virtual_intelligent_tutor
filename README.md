# Intelligent Virtual Tutor
Intelligent Virtual Tutor is an interactive system that provides a dynamic and adaptive learning to different students by adapting the learning process to the student. This application combines Deep Knowledge Tracing algorithm with the Expectimax in order to model the student knowledge and suggest the most suitable for the student exercise. 
Specifically the DKT module is trained on the dataset provided by HackerRank for a challenge. 

### Algorithm used  
Virtual Tutor consist of three modules: <br/>
**__Knowledge Tracing Module:__**  LSTM network, that is predicting the probability of solving the exercise of a student basing on the past performance.
 <br/>
**Sequence constructor:** 
A search module that investigates the probabilities of solving the exercise for a given set of exercises and picks the one that increases the probabilities the most.

![alt text](https://github.com/erytheis/virtual_intelligent_tutor/blob/master/architecture.png)

### How to run

```
$ python main.py
```

Main file runs 3 experiments: 
1) Average probability of solving exercises for a high performing students. The rank of a student can be changed in the ```main.py  ```
2) Average probability of solving exercises for a low performing students. The rank of a student can be changed in the ```main.py  ```
3) Expectimax prediction for a custom hisotry of submission

### Requirements
```
tensorflow
pandas
numpy
scikit-learn
```

### References and credits
 [DKT+ implementation by Chun-Kit Yeung and Dit-Yan Yeung](https://github.com/ckyeungac/deep-knowledge-tracing-plus) <br />
 [DKT implementation by Mohammad Khajah ](https://github.com/mmkhajah/dkt/blob/master/dkt.py)<br />
 [Hackerrank dataset of submission](https://www.hackerrank.com/contests/machine-learning-codesprint/challenges/hackerrank-challenge-recommendation)


