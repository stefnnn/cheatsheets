---
title: Yaml
category: Markup
layout: 2017/sheet
prism_languages: [yaml]
---

### Lists

```yaml
# A list of tasty fruits
- Apple
- Orange
- Strawberry
- Mango
...
```


### Dictionaries

```yaml
# An employee record
martin:
  name: Martin D'vloper
  job: Developer
  skill: hobbyist
```

### Abbreviated Lists / Dictionaries

```yaml
['Apple', 'Orange', 'Strawberry', 'Mango']
martin: {name: Martin D'vloper, job: Developer, skill: Elite}
```

### Multiline strings

```yaml
include_newlines: |
  exactly as you see
  will appear these three
  lines of poetry

fold_newlines: >
  this is really a
  single line of text
  despite appearances
```

### Inheritance

```yaml
parent: &defaults
  a: 2
  b: 3

child:
  <<: *defaults
  b: 4
```

### Reference content

```yaml
values: &ref
  - These values
  - will be reused below
  
other_values:
  <<: *ref
```
