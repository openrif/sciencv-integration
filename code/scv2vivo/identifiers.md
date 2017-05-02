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

#### _orcid uri_
From column: _profile / identification / Unfold: idtype / orcid / Values_
``` python
orcid = getValue("Values")
if orcid:
    return "http://orcid.org/" + orcid
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Values_ | `vivo:eRACommonsId` | `foaf:Person1`|
| _Values_ | `vivo:scopusId` | `foaf:Person1`|
| _Values_ | `vivo:researcherId` | `foaf:Person1`|
| _orcid uri_ | `uri` | `owl:Thing1`|
| _person uri_ | `uri` | `foaf:Person1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `foaf:Person1` | `vivo:orcidId` | `owl:Thing1`|
