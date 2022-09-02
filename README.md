# Experimental Results
|                            Model                             |            ROUGE-L             |             BLEU4              |
| :----------------------------------------------------------: | :----------------------------: | :----------------------------: |
|                 ProphetNet(Qi et al., 2020)                  |             52.26              |             23.91              |
|                  UNILMv2(Bao et al., 2020)                   |             51.97              |             24.43              |
|              Recurrent BERT(Chan and Fan, 2020)              |             47.07              |             19.14              |
|            ProphetNet+ASGEN(Back et al., 2021)\*             |           **52.80**            |             24.40              |
|                    IGND(Fei et al., 2021)                    |             48.94              |             20.33              |
| $\color{rgb(255,0,0)}{ERNIE-GEN-large (Xiao et al., 2020)^\\# }$ | $\color{rgb(255,0,0)}{41.38 }$ | $\color{rgb(255,0,0)}{17.56 }$ |
|    $\color{rgb(255,0,0)}{Bart-base (Lewis et al., 2019)}$    | $\color{rgb(255,0,0)}{47.68}$  | $\color{rgb(255,0,0)}{23.02}$  |
|   $\color{rgb(255,0,0)}{Bart-large (Lewis et al., 2019)}$    | $\color{rgb(255,0,0)}{49.69}$  | $\color{rgb(255,0,0)}{24.73}$  |
|          BART-Base+GraphSAGE(1024)+Copy-net (Ours)           |             47.82              |             22.94              |
|          BART-Large+GraphSAGE(1024)+Copy-net (Ours)          |             49.16              |           **24.82**            |

Table 1:  Experimental results on the SQuAD dataset. Experimental results for the Baseline model are from the corresponding paper. </br>
\*: indicates that we average the results of the two divisions of the SQuAD dataset on the QG task in the ProphetNet+ASGEN paper. </br>$\color{rgb(255,0,0)}{^\\#}$: indicates that we reset *max_src_len=512,max_tgt_len=64,batch_size=8,epoch=10,learning_rate=1e-5,beam_size=5*.




***



|                              Model                               |            ROUGE-L            |             BLEU4             |
|:----------------------------------------------------------------:|:-----------------------------:|:-----------------------------:|
|                    AG-GCN (Jia et al., 2021)                     |             34.24             |             11.96             |
|                  Bart-base (Lewis et al., 2019)                  |             45.39             |             24.48             |
|               Bart-base+Copy-net (Gu et al., 2016)               |             45.52             |             24.55             |
|           Bart-base+GraphSAGE+Undirected-graphs(1024)            |             44.67             |             24.54             |
|     $\color{rgb(255,0,0)}{Bart-large (Lewis et al., 2019)}$      | $\color{rgb(255,0,0)}{45.30}$ | $\color{rgb(255,0,0)}{25.76}$ |
| $\color{rgb(255,0,0)}{ERNIE-GEN-large (Xiao et al., 2020)^\\# }$ | $\color{rgb(255,0,0)}{42.17}$ | $\color{rgb(255,0,0)}{20.54}$ |
|       Bart-base+GraphSAGE+Copy-net+Undirected-graphs(1024)       |           **44.75**           |           **24.90**           |
|      Bart-large+GraphSAGE+Copy-net+Undirected-graphs(1024)       |           **47.15**           |           **27.05**           |

Table 2:  Experimental results on the EQG-RACE dataset.</br>
$\color{rgb(255,0,0)}{^\\#}$ : indicates that we reset *max_src_len=512,max_tgt_len=64,batch_size=8,epoch=10,learning_rate=1e-5,beam_size=5*. 




