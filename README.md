# 声音转换 ——柯南的变声器


<br><br>
<img src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/kenan.jfif"  height="360" width="495">
<br><br>


音色转换是将音频转换成不同音色的音频同时音色信息保持不变就像柯南的变声器一样。我们提出了any2many的音色转换算法既可以将任意人的声音转换成固定的几种音色，同时可以支持多语言的音色转换。模型训练的数据我们选择了中文，英语和德语。音频样本如下：

|  |音频|
-|:-:|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/target/aixiang.wav"  controls > </audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/target/ljs.wav"  controls > </audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/target/german.wav"  controls > </audio>|


<br><br>


中文测试

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/chinese/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/chinese/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/chinese/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/chinese/german.wav" controls ></audio>|

<br><br>

英语测试

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/english/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/english/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/english/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/english/german.wav" controls ></audio>|

<br><br>

德语测试

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/german/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/german/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/german/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/german/german.wav" controls ></audio>|

<br><br>
多语言数据训练的模型在未见过的语言上也可以做音色转换

<br>
日语测试

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/japan/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/japan/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/japan/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/japan/german.wav" controls ></audio>|

<br><br>

西班牙语测试

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/spanish/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/spanish/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/spanish/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/spanish/german.wav" controls ></audio>|


<br><br>
模型还有很强的去背景噪音的能力
|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/noise/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/noise/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/noise/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/data/noise/german.wav" controls ></audio>|

<br><br>
预训练加微调，大数据对模型进行训练让模型能够学习到音频合成的能力，并通过少量的数据对模型进行微调使模型在音色转换上也有不错的效果，我们从训练数据的三个不同音色音频数据中各抽取了三千条数据在预训练模型上进行微调，效果如下，
<br><br>
中文

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/chinese/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/chinese/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/chinese/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/chinese/german.wav" controls ></audio>|

<br><br>
英文

|  |name|
-|:-:|
原始音频|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/english/target.wav" controls ></audio>|
中文男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/english/aixiang.wav" controls ></audio>|
英文女生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/english/ljs.wav" controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/raw/main/few/english/german.wav" controls ></audio>|