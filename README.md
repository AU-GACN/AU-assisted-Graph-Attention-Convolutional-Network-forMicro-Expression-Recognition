# AU-assisted-Graph-Attention-Convolutional-Network-forMicro-Expression-Recognition

----
## Overall Results
LOSO validation
> CASME II (3 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.610|0.253|
|ELRCN|0.623|0.342|
|CapsuleNet|0.568|0.347|
|MER-GCN|0.544|0.303|
|**AU-GACN+AU-ICGAN**|0.712(+8.9%)|0.355(+0.8%)|

> CASME II (7 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.368|0.132|
|ELRCN|0.443|0.325|
|CapsuleNet|0.331|0.194|
|MER-GCN|0.405|0.163|
|**AU-GACN+AU-ICGAN**|0.405(+11.8%)|0.394(+6.9%)|

> SAMM (3 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.676|0.271|
|ELRCN|0.691|0.272|
|CapsuleNet|0.575|0.392|
|MER-GCN|0.534|0.283|
|**AU-GACN+AU-ICGAN**|0.702(+1.1%)|0.433(+4.1%)|

> SAMM (8 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.289|0.094|
|ELRCN|0.358|0.066|
|CapsuleNet|0.259|0.111|
|MER-GCN|0.294|0.010|
|**AU-GACN+AU-ICGAN**|0.523(+16.5%)|0.357(+24.5%)|

LOVO validation
> CASME II (3 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.607|0.398|
|ELRCN|0.609|0.429|
|CapsuleNet|0.582|0.356|
|MER-GCN|0.532|0.412|
|**AU-GACN+AU-ICGAN**|0.634(+2.5%)|0.521(+9.2%)|

> CASME II (7 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.407|0.184|
|ELRCN|0.396|0.197|
|CapsuleNet|0.331|0.155|
|MER-GCN|0.324|0.173|
|**AU-GACN+AU-ICGAN**|0.519(+11.2%)|0.424(+22.7%)|

> SAMM (3 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.694|0.424|
|ELRCN|0.682|0.227|
|CapsuleNet|0.592|0.384|
|MER-GCN|0.542|0.257|
|**AU-GACN+AU-ICGAN**|0.732(+2.7%)|0.454(+3.0%)|

> SAMM (8 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.384|0.149|
|ELRCN|0.359|0.066|
|CapsuleNet|0.266|0.158|
|MER-GCN|0.273|0.108|
|**AU-GACN+AU-ICGAN**|0.426(+16.5%)|0.228(+7.0%)|

## cross-database 

>CASME II => SMIC

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.314|0.190|
|CapsuleNet|0.322|0.152|
|MER-GCN|0.367|0.272|
|**AU-GACN+AU-ICGAN**|0.344(-2.3%)|0.319(+4.7%)|

>SAMM => SMIC

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.325|0.190|
|CapsuleNet|0.324|0.179|
|MER-GCN|0.361|0.178|
|**AU-GACN+AU-ICGAN**|0.451(+9.0%)|0.309(+11.9%)|

## The impact of data augmentation

LOSO validation
>CASME II (7 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.368|0.132|
|STCNN|0.411(+4.3%)|0.253(+12.1%)|
|CapsuleNet|0.331|0.194|
|CapsuleNet + AI-ICGAN|0.368(+3.7%)|0.267(+7.3%)|
|MER-GCN|0.405|0.163|
|MER-GCN+AU-ICGAN|0.441(+3.6%)|0.181(+1.8%)|
|AU-GACN|0.492|0.273|
|**AU-GACN+AU-ICGAN**|0.561(+6.9%)|0.394(+11.9%)|

>SAMM (8 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.289|0.094|
|STCNN|0.367(+7.8%)|0.167(+7.3%)|
|CapsuleNet|0259|0.111|
|CapsuleNet + AI-ICGAN|0.275(+1.6%)|0.193(+8.2%)|
|MER-GCN|0.294|0.010|
|MER-GCN|0.328(+3.6%)|0.124(+11.4%)|
|AU-GACN|0.489|0.310|
|**AU-GACN+AU-ICGAN**|0.523(+3.4%)|0.357(4.7%)|


LOVO validation
>CASME II (7 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.407|0.184|
|STCNN+AU-ICGAN|0.403(-0.4%)|0.273(+8.9%)|
|CapsuleNet|0.324|0.155|
|CapsuleNet + AI-ICGAN|0.338(+1.4%)|0.257(+10.2%)|
|MER-GCN|0.398|0.173|
|MER-GCN+AU-ICGAN|0.439(+4.1%)|0.186(+1.3%)|
|AU-GACN|0.420|0.347|
|**AU-GACN+AU-ICGAN**|0.519(+9.9%)|0.424(+7.7%)|

>SAMM (8 categories)

| Method | ACC | F1-score|
|----|----|----|
|STCNN|0.384|0.149|
|STCNN+AU-ICGAN|0.383(-0.1%)|0.159(+1.0%)|
|CapsuleNet|0.266|0.158|
|CapsuleNet + AI-ICGAN|0.259(-0.67)|0.161(+0.3%)|
|MER-GCN|0.273|0.108|
|MER-GCN+AU-ICGAN|0.344(+7.1%)|0.118(+1.0%)|
|AU-GACN|0.409|0.212|
|**AU-GACN+AU-ICGAN**|0.426(+1.7%)|0.228(1.6%)|
