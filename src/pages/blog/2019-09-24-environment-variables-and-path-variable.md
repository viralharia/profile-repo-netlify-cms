---
templateKey: blog-post
title: Environment variables and Path variable
date: 2019-09-24T08:11:33.626Z
description: Environment variables and Path variable
featuredpost: true
featuredimage: /img/meeting-space.png
tags:
  - environmentVariable
  - pathVariable
---
## Get all the Environment variables
```command
SET
```
The above command will also give the value of `PATH` variable.

## Get the PATH variable value
```command
path
```

## Updating the PATH variable temporary
```command
setx path "%path%;c:\directoryPath"
```
