# Dacon_KNLI

## 2022-02-01

bert classification klue/bert model, best_loss model 5fold

0.742



## 2022-02-02

- sentence bert using u, v, |u-v|
  - 0.61



## 2022-02-03

1

- bert classification klue/bert model, best_acc model 5fold, 
- Adam

2

- auto model KoELECTRA-Base
- AdamW(correct_bias = False)



## 2022-02-04

1

0.83

- electra v3 adamw(1e-5, correct_bias=False), best_acc model 5fold

- ```
  1   Average training loss: 0.4913
    Accuracy: 0.8160
  100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.14it/s]
    0%|                                                                                         | 0/2500 [00:00<?, ?it/s]
  model1 saved
  1   Average valid loss: 0.4784
    Accuracy: 0.8516
  100%|██████████████████████████████████████████████████████████████████████████████| 2500/2500 [09:33<00:00,  4.36it/s]
    0%|▎                                                                                 | 2/625 [00:00<00:45, 13.74it/s]
  2   Average training loss: 0.2919
    Accuracy: 0.9120
  100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.13it/s]
    0%|                                                                                         | 0/2500 [00:00<?, ?it/s]
  model1 saved
  2   Average valid loss: 0.5145
    Accuracy: 0.8722
  100%|██████████████████████████████████████████████████████████████████████████████| 2500/2500 [09:33<00:00,  4.36it/s]
    0%|▎                                                                                 | 2/625 [00:00<00:45, 13.74it/s]
  3   Average training loss: 0.1930
    Accuracy: 0.9508
  100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.11it/s]
  3   Average valid loss: 0.6374
    Accuracy: 0.8650
  ```

2.

0.83

electra v3 adam(2e-5), best_acc model 5fold

```
1   Average training loss: 0.5118
  Accuracy: 0.8087
100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.07it/s]
  0%|                                                                                         | 0/2500 [00:00<?, ?it/s]
model1 saved
1   Average valid loss: 0.4886
  Accuracy: 0.8548
100%|██████████████████████████████████████████████████████████████████████████████| 2500/2500 [09:47<00:00,  4.25it/s]
  0%|▎                                                                                 | 2/625 [00:00<00:45, 13.74it/s]
2   Average training loss: 0.2970
  Accuracy: 0.9153
100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.09it/s]
  0%|                                                                                         | 0/2500 [00:00<?, ?it/s]
model1 saved
2   Average valid loss: 0.5668
  Accuracy: 0.8630
100%|██████████████████████████████████████████████████████████████████████████████| 2500/2500 [09:46<00:00,  4.26it/s]
  0%|▎                                                                                 | 2/625 [00:00<00:45, 13.64it/s]
3   Average training loss: 0.1894
  Accuracy: 0.9546
100%|████████████████████████████████████████████████████████████████████████████████| 625/625 [00:44<00:00, 14.11it/s]
model1 saved
3   Average valid loss: 0.6407
  Accuracy: 0.8668
```



4. roberta large

```
1   Average training loss: 0.4982
  Accuracy: 0.7962
100%|██████████| 157/157 [00:37<00:00,  4.18it/s]
model1 saved
1   Average valid loss: 0.3384
  Accuracy: 0.8792
100%|██████████| 625/625 [07:48<00:00,  1.33it/s]
2   Average training loss: 0.2284
  Accuracy: 0.9252
100%|██████████| 157/157 [00:37<00:00,  4.17it/s]
model1 saved
2   Average valid loss: 0.3157
  Accuracy: 0.8985
100%|██████████| 625/625 [07:48<00:00,  1.33it/s]
3   Average training loss: 0.1352
  Accuracy: 0.9606
100%|██████████| 157/157 [00:37<00:00,  4.17it/s]
3   Average valid loss: 0.3788
  Accuracy: 0.8983
```



## 2022-02-06

teacher electra student roberta-large

0.863

```
1   Average training loss: 2.2603
  Accuracy: 0.8116
100%|██████████| 157/157 [00:37<00:00,  4.16it/s]
model1 saved
1   Average valid loss: 0.5959
  Accuracy: 0.8863
100%|██████████| 625/625 [08:02<00:00,  1.30it/s]
2   Average training loss: 0.8959
  Accuracy: 0.9163
100%|██████████| 157/157 [00:37<00:00,  4.16it/s]
model1 saved
2   Average valid loss: 0.5404
  Accuracy: 0.8939
100%|██████████| 625/625 [08:02<00:00,  1.30it/s]
3   Average training loss: 0.6316
  Accuracy: 0.9392
100%|██████████| 157/157 [00:37<00:00,  4.16it/s]
model1 saved
3   Average valid loss: 0.5997
  Accuracy: 0.8961
```



2. xavier normal

   ```
   1   Average training loss: 0.4814
     Accuracy: 0.8183
   100%|██████████| 157/157 [00:37<00:00,  4.15it/s]
   model1 saved
   1   Average valid loss: 0.3163
     Accuracy: 0.8927
   100%|██████████| 625/625 [08:01<00:00,  1.30it/s]
   2   Average training loss: 0.2242
     Accuracy: 0.9293
   100%|██████████| 157/157 [00:37<00:00,  4.15it/s]
   model1 saved
   2   Average valid loss: 0.3162
     Accuracy: 0.8961
   ```



3. xavier_normal + bn init



## 2022-02-07

0.874

backtranslation이용 roberta-large



## 2022-02-08

0.874

roberta-large, self-explainable, 논문에서 제안한 loss가 아닌 평범한 ce loss 사용

