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
| _addresstype_ | `rdfs:label` | `vcard:URL1`|
| _content_ | `vcard:url` | `vcard:URL1`|
| _givennames_ | `vcard:givenName` | `vcard:Name1`|
| _person uri_ | `uri` | `foaf:Person1`|
| _prefix_ | `vcard:honorificPrefix` | `vcard:Name1`|
| _presentedname_ | `vcard:formattedName` | `vcard:FormattedName1`|
| _salutation_ | `vcard:title` | `vcard:Title1`|
| _suffix_ | `vcard:honorificSuffix` | `vcard:Name1`|
| _surname_ | `vcard:familyName` | `vcard:Name1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `foaf:Person1` | `obo:ARG_2000028` | `vcard:Individual1`|
| `vcard:Individual1` | `vcard:hasFormattedName` | `vcard:FormattedName1`|
| `vcard:Individual1` | `vcard:hasName` | `vcard:Name1`|
| `vcard:Individual1` | `vcard:hasTitle` | `vcard:Title1`|
| `vcard:Individual1` | `vcard:hasURL` | `vcard:URL1`|
