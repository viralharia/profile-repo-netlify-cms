---
templateKey: blog-post
title: Linux commands
date: '2019-11-11 12:06'
featuredpost: true
featuredimage: /img/chemex.jpg
tags:
  - linux
---
### base64 encoding and decoding
**Encoding**
```
base64 data.txt

echo 'this is sanfoundry linux tutorial' | base64

base64 data.txt > data.b64
```
**Decoding**
```
base64 -d data.b64 > data.txt

echo 'dGhpcyBpcyBzYW5mb3VuZHJ5IGxpbnV4IHR1dG9yaWFsCg==' | base64 -d
```
***
### To permanently set an environment variable
- Open the terminal and run the below command

```
gedit ~/.profile
```
- Add the command to the bottom of the file.
- Save and close gedit.

***
