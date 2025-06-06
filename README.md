# Geophysical Waveform Inversion
Develop physics-guided machine learning models to solve full-waveform inversion problems

## Basics
### Overview
このコンペティションでは、地震波形データから速度マップなどの**地下物性**を推定することが求められます。
このプロセスは**全波形インバージョン（Full Waveform Inversion, FWI）** として知られており、より高精度かつ効率的な地震解析を可能にし、さまざまな分野での応用価値を高めることが期待されています。


### Description
医師が超音波画像を解析する場面を想像してみてください。ただぼんやりとした輪郭を見るのではなく、正確な診断に必要な、より鮮明で詳細な画像を得ようとしています。これは、地球内部の構造を可視化しようとする地球物理学者が直面している課題と同じです。地中には、重要な資源や潜在的な危険、そして地球の歴史を解き明かす手がかりが隠されています。これらを十分に理解し有効活用するには、より高精度な地下構造のイメージングが不可欠です。

**全波形インバージョン（Full Waveform Inversion, FWI）** は、これらの秘密を解き明かす鍵となる技術です。FWIは、エネルギー探査や二酸化炭素の地中貯留、医療用超音波診断、高度な材料検査などにおいて極めて重要であり、地震波の波形全体を解析することで、地下の詳細な構造像を構築しようとするものです。しかし、現実のデータにはノイズが多く、この手法の活用には大きな障壁があります。

従来の物理モデルに基づくアプローチは高精度ですが、計算に非常に時間がかかり、信号が弱いノイズの多いデータに対しては誤差が生じやすいという欠点があります。一方で、機械学習だけに頼る手法は処理速度が速いものの、大量のラベル付きデータを必要とし、新たな未知の「信号」に対してはうまく対応できないことが多いです。

このコンペティションでは、物理学と機械学習の両者を融合させてFWIを進化させることが求められます。この課題に成功すれば、地下資源探査だけでなく、医療診断や非破壊検査など、精密なイメージングが求められるさまざまな分野に革新をもたらす可能性があります。

### train_samples
<pre>
/kaggle/input/waveform-inversion
├── sample_submission.csv
├── test
└── train_samples
    ├── CurveFault_A/
    │   ├── seis2_1_0.npy
    │   ├── seis4_1_0.npy
    │   ├── vel2_1_0.npy
    │   └── vel4_1_0.npy
    ├── CurveFault_B/
    │   ├── seis6_1_0.npy
    │   ├── seis8_1_0.npy
    │   ├── vel6_1_0.npy
    │   └── vel8_1_0.npy
    ├── CurveVel_A/
    │   ├── data/
    │   │   ├── data1.npy
    │   │   └── data2.npy
    │   └── model/
    │       ├── model1.npy
    │       └── model2.npy
    ├── CurveVel_B/
    │   ├── data/
    │   │   ├── data1.npy
    │   │   └── data2.npy
    │   └── model/
    │       ├── model1.npy
    │       └── model2.npy
    ├── FlatFault_A/
    │   ├── seis2_1_0.npy
    │   ├── seis4_1_0.npy
    │   ├── vel2_1_0.npy
    │   └── vel4_1_0.npy
    ├── FlatFault_B/
    │   ├── seis6_1_0.npy
    │   ├── seis8_1_0.npy
    │   ├── vel6_1_0.npy
    │   └── vel8_1_0.npy
    ├── FlatVel_A/
    │   ├── data/
    │   │   ├── data1.npy
    │   │   └── data2.npy
    │   └── model/
    │       ├── model1.npy
    │       └── model2.npy
    ├── FlatVel_B/
    │   ├── data/
    │   │   ├── data1.npy
    │   │   └── data2.npy
    │   └── model/
    │       ├── model1.npy
    │       └── model2.npy
    ├── Style_A/
    │   ├── data/
    │   │   ├── data1.npy
    │   │   └── data2.npy
    │   └── model/
    │       ├── model1.npy
    │       └── model2.npy
    └── Style_B/
        ├── data/
        │   ├── data1.npy
        │   └── data2.npy
        └── model/
            ├── model1.npy
            └── model2.npy
</pre>

|name|Explanation|
|----|----|
|rating|録音の質を表す(A,B,C,D,Eの5段階)|
|playback_sed|...|
|ebird_code|名前。nunique=264|

### submission.csv 

## Features
|Name|shape (feat only)|size(MB)|Detail|

## Paper
|No.|Status|Name|Detail|Date|Url|
|---|---|---|---|---|---|


## Log
### 20250606(Fri.)
- join!!
- [チュートリアル](https://www.kaggle.com/code/suirikais/waveform-inversion-kaggle-competition-tutorial)　やった
