# 6.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _person uri_
From column: _profile / identification / name / givennames_
``` python
name = getValue("givennames") + getValue("surname")
return personNameUri(name)
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _person uri_ | `uri` | `foaf:Person1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
