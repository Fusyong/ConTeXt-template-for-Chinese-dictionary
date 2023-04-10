一个ConTeXt中文词典模版，主要解决**版面元素和排式的自动化**问题，不解决：

* 词典原稿的解析、加样式；
* 原稿与成品校验的自动化；
* 美术上的样式精调。

当另案处理。

## 样张版权

本项目样张中的内容均选自《现代汉语词典》，所有权利归属于其著作权人；
本人不拥有任何权利，仅用作研究和学习排版样式之模式材料。
您如有著作权异议，请联系我： aahuaang@gmail.com

## 功能、问题和TODO

* [x] 页眉的字头列表
* [x] 页眉的音节起止
  * [ ] 只保留第一个音节
* [ ] 音节表
* [ ] 部首检字表
* [ ] 检字表
* [ ] 难检字笔画索引
* [ ] 常用排式
  * [x] 字头（单字词）主字头
    * [ ] 第一段第二行的缩进有误
    * [ ] 上标
  * [ ] 繁体字
  * [ ] 异体字
  * [x] 词头（多字词）
    * [ ] 上标
  * [ ] 例词例句
  * [ ] 词性标记
  * [ ] 拼音
  * [ ] 异形字词（“同”）
  * [ ] 同音同形条目（数字上标）
  * [ ] 同形异音条目（“另见”）
  * [ ] 儿化韵尾


<!--

## 读取json

```lua
local tmp = [[ { "t\nt t" : "foo bar", "a" : true, "b" : [ 123 , 456E-10, { "a" : true, "b" : [ 123 , 456 ] } ] } ]]
tmp = json.tolua(tmp)
inspect(tmp)
tmp = json.tostring(tmp,true)
inspect(tmp)
tmp = json.tolua(tmp)
inspect(tmp)
tmp = json.tostring(tmp)
inspect(tmp)
inspect(json.tostring(true))

local s = [[\foo"bar"]]
local j = json.tostring { s = s }
local l = json.tolua(j)
inspect(j)
inspect(l)
print(s==l.s)

if not package.loaded.json then
    package.loaded.json = json
end
```

\ci
{}
{}
{}
{}

\zi
{}
{}
{}
{}

  -->