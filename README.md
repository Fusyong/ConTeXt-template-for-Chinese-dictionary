
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