# 声音转换 ——柯南的变声器
<br><br>
<img src="https://github.com/R-ookie/R-ookie.github.io/blob/main/data/kenan.jfif"  height="360" width="495">
<br><br>


音色转换是将音频转换成不同音色的音频同时银色信息保持不变就像柯南的变声器一样。我们提出了any2many的音色转换算法既可以将任意人的声音转换成固定的几种音色，同时可以支持多语言的音色转换。模型训练的数据我们选择了中文，英语和德语。音频样本如下：

|  |音频|
-|:-:|
中文男生|<audio src= [1] controls ></audio>|
中文女生|<audio src= [2] controls ></audio>|
英文女生|<audio src= [3] controls ></audio>|
德语男生|<audio src="https://github.com/R-ookie/R-ookie.github.io/blob/main/data/german.wav"> </audio>|


<br><br>


中文测试

|  |name|name|
-|:-:|:-:|
原始音频|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文男生|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文女生|<audio src=[2] controls ></audio>|<audio src=[1] controls ></audio>
英文女生|<audio src=[3] controls ></audio>|<audio src=[1] controls ></audio>
德语男生|<audio src=[5] controls ></audio>|<audio src=[1] controls ></audio>

<br><br>

英语测试

|  |name|name|
-|:-:|:-:|
原始音频|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文男生|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文女生|<audio src=[2] controls ></audio>|<audio src=[1] controls ></audio>
英文女生|<audio src=[3] controls ></audio>|<audio src=[1] controls ></audio>
德语男生|<audio src=[4] controls ></audio>|<audio src=[1] controls ></audio>

<br><br>

德语测试

|  |name|name|
-|:-:|:-:|
原始音频|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文男生|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文女生|<audio src=[2] controls ></audio>|<audio src=[1] controls ></audio>
英文女生|<audio src=[3] controls ></audio>|<audio src=[1] controls ></audio>
德语男生|<audio src=[4] controls ></audio>|<audio src=[1] controls ></audio>

<br><br>
多语言数据训练的模型在未见过的语言上也可以做音色转换

<br>
日语测试

|  |name|name|
-|:-:|:-:|
原始音频|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文男生|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文女生|<audio src=[2] controls ></audio>|<audio src=[1] controls ></audio>
英文女生|<audio src=[3] controls ></audio>|<audio src=[1] controls ></audio>
德语男生|<audio src=[4] controls ></audio>|<audio src=[1] controls ></audio>

<br><br>

西班牙语测试

|  |name|name|
-|:-:|:-:|
原始音频|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文男生|<audio src=[1] controls ></audio>|<audio src=[1] controls ></audio>
中文女生|<audio src=[2] controls ></audio>|<audio src=[1] controls ></audio>
英文女生|<audio src=[3] controls ></audio>|<audio src=[1] controls ></audio>
德语男生|<audio src=[4] controls ></audio>|<audio src=[1] controls ></audio>