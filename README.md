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

```
1   Average training loss: 0.4580
  Accuracy: 0.8209
100%|██████████| 157/157 [00:58<00:00,  2.67it/s]
model1 saved
1   Average valid loss: 0.2875
  Accuracy: 0.8953
100%|██████████| 625/625 [09:36<00:00,  1.08it/s]
2   Average training loss: 0.2177
  Accuracy: 0.9284
100%|██████████| 157/157 [00:59<00:00,  2.64it/s]
2   Average valid loss: 0.2901
  Accuracy: 0.8945
100%|██████████| 625/625 [09:34<00:00,  1.09it/s]
3   Average training loss: 0.1327
  Accuracy: 0.9620
100%|██████████| 157/157 [00:59<00:00,  2.63it/s]
model1 saved
3   Average valid loss: 0.3758
  Accuracy: 0.9011
```

```
kaggle tpu

!curl https://raw.githubusercontent.com/pytorch/xla/master/contrib/scripts/env-setup.py -o pytorch-xla-env-setup.py
!python pytorch-xla-env-setup.py --apt-packages libomp5 libopenblas-dev

!pip install https://storage.googleapis.com/tpu-pytorch/wheels/torch_xla-1.6-cp37-cp37m-linux_x86_64.whl
!pip install torch==1.6

import torch_xla
import torch_xla.core.xla_model as xm
```





self train  데이터 추가 후 ce + reg loss 사용시



```
1   Average training loss: 0.4695
  Accuracy: 0.8216
100%|██████████| 175/175 [01:06<00:00,  2.64it/s]
model1 saved
1   Average valid loss: 0.3009
  Accuracy: 0.8945
100%|██████████| 700/700 [10:47<00:00,  1.08it/s]
2   Average training loss: 0.2208
  Accuracy: 0.9297
100%|██████████| 175/175 [01:05<00:00,  2.67it/s]
2   Average valid loss: 0.3849
  Accuracy: 0.8834
100%|██████████| 700/700 [10:47<00:00,  1.08it/s]
3   Average training loss: 0.1414
  Accuracy: 0.9588
100%|██████████| 175/175 [01:05<00:00,  2.66it/s]
model1 saved
3   Average valid loss: 0.3795
  Accuracy: 0.8973
```



## 2022-02-09

self-explain, ce - reg loss

0.883

```
1   Average training loss: 0.1291
  Accuracy: 0.8208
100%|██████████| 175/175 [01:06<00:00,  2.65it/s]
model1 saved
1   Average valid loss: 0.3065
  Accuracy: 0.8934
100%|██████████| 700/700 [10:48<00:00,  1.08it/s]

2   Average training loss: -0.7642
  Accuracy: 0.9228
100%|██████████| 175/175 [01:05<00:00,  2.67it/s]
model1 saved
2   Average valid loss: 0.3388
  Accuracy: 0.8989
100%|██████████| 700/700 [10:49<00:00,  1.08it/s]

3   Average training loss: -0.8565
  Accuracy: 0.9576
100%|██████████| 175/175 [01:05<00:00,  2.65it/s]
3   Average valid loss: 0.4302
  Accuracy: 0.8978
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.bias', 'lm_head.decoder.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.layer_norm.weight', 'lm_head.dense.weight', 'lm_head.decoder.weight']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------2----------------------
100%|██████████| 700/700 [10:46<00:00,  1.08it/s]

1   Average training loss: 0.3452
  Accuracy: 0.8214
100%|██████████| 175/175 [01:06<00:00,  2.64it/s]
model2 saved
1   Average valid loss: 0.3173
  Accuracy: 0.8914
100%|██████████| 700/700 [10:45<00:00,  1.08it/s]

2   Average training loss: -0.7611
  Accuracy: 0.9241
100%|██████████| 175/175 [01:06<00:00,  2.62it/s]
model2 saved
2   Average valid loss: 0.3358
  Accuracy: 0.9000
100%|██████████| 700/700 [10:45<00:00,  1.09it/s]

3   Average training loss: -0.8605
  Accuracy: 0.9588
100%|██████████| 175/175 [01:06<00:00,  2.64it/s]
model2 saved
3   Average valid loss: 0.3811
  Accuracy: 0.9009
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.bias', 'lm_head.decoder.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.layer_norm.weight', 'lm_head.dense.weight', 'lm_head.decoder.weight']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------3----------------------
100%|██████████| 700/700 [10:47<00:00,  1.08it/s]

1   Average training loss: 0.2217
  Accuracy: 0.8215
100%|██████████| 175/175 [01:06<00:00,  2.64it/s]
model3 saved
1   Average valid loss: 0.3187
  Accuracy: 0.8878
100%|██████████| 700/700 [10:47<00:00,  1.08it/s]

2   Average training loss: -0.7217
  Accuracy: 0.9184
100%|██████████| 175/175 [01:05<00:00,  2.65it/s]
2   Average valid loss: 0.3907
  Accuracy: 0.8617
100%|██████████| 700/700 [10:47<00:00,  1.08it/s]

3   Average training loss: -0.7846
  Accuracy: 0.9412
100%|██████████| 175/175 [01:06<00:00,  2.65it/s]
model3 saved
3   Average valid loss: 0.3887
  Accuracy: 0.8884
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.bias', 'lm_head.decoder.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.layer_norm.weight', 'lm_head.dense.weight', 'lm_head.decoder.weight']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------4----------------------
100%|██████████| 700/700 [10:48<00:00,  1.08it/s]

1   Average training loss: 0.0888
  Accuracy: 0.8206
100%|██████████| 175/175 [01:06<00:00,  2.64it/s]
model4 saved
1   Average valid loss: 0.2812
  Accuracy: 0.8991
100%|██████████| 700/700 [10:46<00:00,  1.08it/s]

2   Average training loss: -0.7717
  Accuracy: 0.9265
100%|██████████| 175/175 [01:05<00:00,  2.66it/s]
model4 saved
2   Average valid loss: 0.3018
  Accuracy: 0.9069
100%|██████████| 700/700 [10:46<00:00,  1.08it/s]

3   Average training loss: -0.8544
  Accuracy: 0.9582
100%|██████████| 175/175 [01:05<00:00,  2.67it/s]
3   Average valid loss: 0.3419
  Accuracy: 0.8996
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.bias', 'lm_head.decoder.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.layer_norm.weight', 'lm_head.dense.weight', 'lm_head.decoder.weight']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------5----------------------
100%|██████████| 700/700 [10:45<00:00,  1.08it/s]

1   Average training loss: -0.0591
  Accuracy: 0.8279
100%|██████████| 175/175 [01:05<00:00,  2.66it/s]
model5 saved
1   Average valid loss: 0.3396
  Accuracy: 0.8876
100%|██████████| 700/700 [10:48<00:00,  1.08it/s]

2   Average training loss: -0.7645
  Accuracy: 0.9260
100%|██████████| 175/175 [01:05<00:00,  2.67it/s]
2   Average valid loss: 0.3465
  Accuracy: 0.8813
100%|██████████| 700/700 [10:50<00:00,  1.08it/s]

3   Average training loss: -0.8448
  Accuracy: 0.9550
100%|██████████| 175/175 [01:06<00:00,  2.63it/s]
model5 saved
3   Average valid loss: 0.3914
  Accuracy: 0.8918
```



2.self-explain, ce + reg loss, best_acc

0.884





init_params1

```
1   Average training loss: 0.4908
  Accuracy: 0.8101
100%|██████████| 222/222 [01:25<00:00,  2.61it/s]
model1 saved
1   Average valid loss: 0.3785
  Accuracy: 0.8663
100%|██████████| 888/888 [13:51<00:00,  1.07it/s]
2   Average training loss: 0.2122
  Accuracy: 0.9280
100%|██████████| 222/222 [01:24<00:00,  2.62it/s]
model1 saved
2   Average valid loss: 0.3931
  Accuracy: 0.8821
```





init_params를 줬을 때 결과2

```
1   Average training loss: 0.4908
  Accuracy: 0.8091
100%|██████████| 222/222 [01:27<00:00,  2.55it/s]
model1 saved
1   Average valid loss: 0.4011
  Accuracy: 0.8581
100%|██████████| 888/888 [13:55<00:00,  1.06it/s]
2   Average training loss: 0.2135
  Accuracy: 0.9291
100%|██████████| 222/222 [01:26<00:00,  2.56it/s]
model1 saved
2   Average valid loss: 0.4464
  Accuracy: 0.8831
100%|██████████| 888/888 [13:55<00:00,  1.06it/s]
3   Average training loss: 0.0913
  Accuracy: 0.9739
100%|██████████| 222/222 [01:26<00:00,  2.56it/s]
model1 saved
3   Average valid loss: 0.5433
  Accuracy: 0.8918
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.layer_norm.bias', 'lm_head.dense.bias', 'lm_head.decoder.weight', 'lm_head.dense.weight', 'lm_head.decoder.bias', 'lm_head.layer_norm.weight', 'lm_head.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------2----------------------
100%|██████████| 888/888 [13:57<00:00,  1.06it/s]
1   Average training loss: 0.5042
  Accuracy: 0.8050
100%|██████████| 222/222 [01:26<00:00,  2.57it/s]
model2 saved
1   Average valid loss: 0.3883
  Accuracy: 0.8598
100%|██████████| 888/888 [13:58<00:00,  1.06it/s]
2   Average training loss: 0.2219
  Accuracy: 0.9248
100%|██████████| 222/222 [01:26<00:00,  2.56it/s]
model2 saved
2   Average valid loss: 0.3812
  Accuracy: 0.8819
100%|██████████| 888/888 [13:55<00:00,  1.06it/s]
3   Average training loss: 0.0936
  Accuracy: 0.9721
100%|██████████| 222/222 [01:26<00:00,  2.55it/s]
model2 saved
3   Average valid loss: 0.5574
  Accuracy: 0.8821
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.layer_norm.bias', 'lm_head.dense.bias', 'lm_head.decoder.weight', 'lm_head.dense.weight', 'lm_head.decoder.bias', 'lm_head.layer_norm.weight', 'lm_head.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------3----------------------
100%|██████████| 888/888 [13:56<00:00,  1.06it/s]
1   Average training loss: 0.4815
  Accuracy: 0.8136
100%|██████████| 222/222 [01:26<00:00,  2.57it/s]
model3 saved
1   Average valid loss: 0.3485
  Accuracy: 0.8768
100%|██████████| 888/888 [13:57<00:00,  1.06it/s]
2   Average training loss: 0.2106
  Accuracy: 0.9308
100%|██████████| 222/222 [01:26<00:00,  2.56it/s]
model3 saved
2   Average valid loss: 0.3905
  Accuracy: 0.8831
100%|██████████| 888/888 [13:57<00:00,  1.06it/s]
3   Average training loss: 0.0871
  Accuracy: 0.9751
100%|██████████| 222/222 [01:26<00:00,  2.55it/s]
model3 saved
3   Average valid loss: 0.5540
  Accuracy: 0.8871
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.layer_norm.bias', 'lm_head.dense.bias', 'lm_head.decoder.weight', 'lm_head.dense.weight', 'lm_head.decoder.bias', 'lm_head.layer_norm.weight', 'lm_head.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------4----------------------
100%|██████████| 888/888 [13:56<00:00,  1.06it/s]
1   Average training loss: 0.5013
  Accuracy: 0.8004
100%|██████████| 222/222 [01:27<00:00,  2.54it/s]
model4 saved
1   Average valid loss: 0.3549
  Accuracy: 0.8684
100%|██████████| 888/888 [13:56<00:00,  1.06it/s]
2   Average training loss: 0.2095
  Accuracy: 0.9286
100%|██████████| 222/222 [01:27<00:00,  2.54it/s]
model4 saved
2   Average valid loss: 0.3603
  Accuracy: 0.8890
100%|██████████| 888/888 [13:56<00:00,  1.06it/s]
3   Average training loss: 0.0912
  Accuracy: 0.9738
100%|██████████| 222/222 [01:27<00:00,  2.53it/s]
3   Average valid loss: 0.5162
  Accuracy: 0.8874
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.layer_norm.bias', 'lm_head.dense.bias', 'lm_head.decoder.weight', 'lm_head.dense.weight', 'lm_head.decoder.bias', 'lm_head.layer_norm.weight', 'lm_head.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.weight', 'roberta.pooler.dense.bias']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------5----------------------
100%|██████████| 888/888 [13:59<00:00,  1.06it/s]
1   Average training loss: 0.4826
  Accuracy: 0.8115
100%|██████████| 222/222 [01:26<00:00,  2.55it/s]
model5 saved
1   Average valid loss: 0.3264
  Accuracy: 0.8778
100%|██████████| 888/888 [14:00<00:00,  1.06it/s]
2   Average training loss: 0.2056
  Accuracy: 0.9317
100%|██████████| 222/222 [01:27<00:00,  2.54it/s]
model5 saved
2   Average valid loss: 0.3766
  Accuracy: 0.8870
100%|██████████| 888/888 [13:59<00:00,  1.06it/s]
3   Average training loss: 0.0917
  Accuracy: 0.9728
100%|██████████| 222/222 [01:27<00:00,  2.54it/s]
model5 saved
3   Average valid loss: 0.4564
  Accuracy: 0.8942
```



max_len = 늘림



```
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.weight', 'lm_head.layer_norm.weight', 'lm_head.decoder.weight', 'lm_head.dense.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.decoder.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.bias', 'roberta.pooler.dense.weight']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------1----------------------
100%|██████████| 1775/1775 [15:14<00:00,  1.94it/s]
1   Average training loss: 0.5067
  Accuracy: 0.8063
100%|██████████| 444/444 [01:25<00:00,  5.21it/s]
model1 saved
1   Average valid loss: 0.4204
  Accuracy: 0.8717
100%|██████████| 1775/1775 [15:13<00:00,  1.94it/s]
2   Average training loss: 0.2312
  Accuracy: 0.9286
100%|██████████| 444/444 [01:25<00:00,  5.17it/s]
model1 saved
2   Average valid loss: 0.4695
  Accuracy: 0.8847
100%|██████████| 1775/1775 [15:08<00:00,  1.95it/s]
3   Average training loss: 0.1037
  Accuracy: 0.9765
100%|██████████| 444/444 [01:25<00:00,  5.22it/s]
model1 saved
3   Average valid loss: 0.6454
  Accuracy: 0.8919
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.weight', 'lm_head.layer_norm.weight', 'lm_head.decoder.weight', 'lm_head.dense.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.decoder.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.bias', 'roberta.pooler.dense.weight']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------2----------------------
100%|██████████| 1775/1775 [15:18<00:00,  1.93it/s]
1   Average training loss: 0.4965
  Accuracy: 0.8150
100%|██████████| 444/444 [01:24<00:00,  5.24it/s]
model2 saved
1   Average valid loss: 0.3913
  Accuracy: 0.8736
100%|██████████| 1775/1775 [15:15<00:00,  1.94it/s]
2   Average training loss: 0.2322
  Accuracy: 0.9278
100%|██████████| 444/444 [01:25<00:00,  5.20it/s]
model2 saved
2   Average valid loss: 0.4314
  Accuracy: 0.8850
100%|██████████| 1775/1775 [15:13<00:00,  1.94it/s]
3   Average training loss: 0.1097
  Accuracy: 0.9739
100%|██████████| 444/444 [01:25<00:00,  5.21it/s]
model2 saved
3   Average valid loss: 0.6335
  Accuracy: 0.8910
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.weight', 'lm_head.layer_norm.weight', 'lm_head.decoder.weight', 'lm_head.dense.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.decoder.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.bias', 'roberta.pooler.dense.weight']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------3----------------------
100%|██████████| 1775/1775 [15:16<00:00,  1.94it/s]
1   Average training loss: 0.4983
  Accuracy: 0.8092
100%|██████████| 444/444 [01:24<00:00,  5.25it/s]
model3 saved
1   Average valid loss: 0.3787
  Accuracy: 0.8681
100%|██████████| 1775/1775 [15:15<00:00,  1.94it/s]
2   Average training loss: 0.2230
  Accuracy: 0.9324
100%|██████████| 444/444 [01:24<00:00,  5.23it/s]
model3 saved
2   Average valid loss: 0.4102
  Accuracy: 0.8823
100%|██████████| 1775/1775 [15:12<00:00,  1.95it/s]
3   Average training loss: 0.0977
  Accuracy: 0.9764
100%|██████████| 444/444 [01:25<00:00,  5.19it/s]
model3 saved
3   Average valid loss: 0.6828
  Accuracy: 0.8838
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.weight', 'lm_head.layer_norm.weight', 'lm_head.decoder.weight', 'lm_head.dense.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.decoder.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.bias', 'roberta.pooler.dense.weight']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------4----------------------
100%|██████████| 1775/1775 [15:13<00:00,  1.94it/s]
1   Average training loss: 0.4939
  Accuracy: 0.8131
100%|██████████| 444/444 [01:26<00:00,  5.16it/s]
model4 saved
1   Average valid loss: 0.4010
  Accuracy: 0.8549
100%|██████████| 1775/1775 [15:14<00:00,  1.94it/s]
2   Average training loss: 0.2275
  Accuracy: 0.9305
100%|██████████| 444/444 [01:25<00:00,  5.19it/s]
model4 saved
2   Average valid loss: 0.5538
  Accuracy: 0.8752
100%|██████████| 1775/1775 [15:07<00:00,  1.96it/s]
3   Average training loss: 0.1057
  Accuracy: 0.9749
100%|██████████| 444/444 [01:25<00:00,  5.18it/s]
model4 saved
3   Average valid loss: 0.6388
  Accuracy: 0.8884
Some weights of the model checkpoint at klue/roberta-large were not used when initializing RobertaModel: ['lm_head.dense.weight', 'lm_head.layer_norm.weight', 'lm_head.decoder.weight', 'lm_head.dense.bias', 'lm_head.layer_norm.bias', 'lm_head.bias', 'lm_head.decoder.bias']
- This IS expected if you are initializing RobertaModel from the checkpoint of a model trained on another task or with another architecture (e.g. initializing a BertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing RobertaModel from the checkpoint of a model that you expect to be exactly identical (initializing a BertForSequenceClassification model from a BertForSequenceClassification model).
Some weights of RobertaModel were not initialized from the model checkpoint at klue/roberta-large and are newly initialized: ['roberta.pooler.dense.bias', 'roberta.pooler.dense.weight']
You should probably TRAIN this model on a down-stream task to be able to use it for predictions and inference.
------------fold no---------5----------------------
100%|██████████| 1775/1775 [15:16<00:00,  1.94it/s]
1   Average training loss: 0.5099
  Accuracy: 0.8042
100%|██████████| 444/444 [01:24<00:00,  5.24it/s]
model5 saved
1   Average valid loss: 0.3474
  Accuracy: 0.8793
100%|██████████| 1775/1775 [15:14<00:00,  1.94it/s]
2   Average training loss: 0.2307
  Accuracy: 0.9283
100%|██████████| 444/444 [01:25<00:00,  5.21it/s]
model5 saved
2   Average valid loss: 0.4678
  Accuracy: 0.8853
100%|██████████| 1775/1775 [15:09<00:00,  1.95it/s]
3   Average training loss: 0.1036
  Accuracy: 0.9751
100%|██████████| 444/444 [01:25<00:00,  5.21it/s]
model5 saved
3   Average valid loss: 0.5758
  Accuracy: 0.8918
```



# 2022-02-16

_1

기존 best_model 것에서 6개 중복데이터 추가, lambda 1.1로 학습

