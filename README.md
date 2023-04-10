一个ConTeXt中文词典模版，主要解决两个问题：

* 排式的自动化；
* 校验的自动化；

不解决：

* 样式美术上的精调；
* 词典原稿的解析、加样式。

## 样张版权

本项目样张中的内容均选自《现代汉语词典》，所有权利归属于其著作权人；
本人不拥有任何权利，仅用作研究和学习排版样式之模式材料。
您如有著作权异议，请联系我： aahuaang@gmail.com

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