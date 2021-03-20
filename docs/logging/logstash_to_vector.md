# Vector from Logstash

As a long time logstash user ive recently been looking at alternatives to broaden my experience and also to deal with any future licensing issues due to logstash now no longer being apache licensed (and no open distro logstash/beats). Naturally FluentD and FluentBit are the main choice here, but they are done to death , I wanted something new and I found [Vector](https://vector.dev/) which is a RUST based log pipeline which looked promising so this is some notes on trying it out coming from logstash

## Introduction

Vector works the like logstash with a 3 stage pipleine. The following table details how they are named

| logstash | vector |
| ----- | ----- |
| input | sources|
| filter | transforms|
| output | sinks |

--- 
## Sources (input)

vector sources are pretty straight forward, the same as you would use for logstash inputs. There are some preconfigured ones for certain solutions ie

* Apache HTTPD
* AWS S3
* Docker 
* MongoDB

These act like "module" in logtsash being ready to use nearly. There are so also more generic ones which you use for most things ie.

* File
* Syslog
* http
* STDIN

[Vector Sources](https://vector.dev/docs/reference/configuration/sources/)

---

## Transforms (fiilter)
---
todo

## Sinks (output)
todo
---
## Wrap up

You can now hail <s>vectron</s> vector

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/icTrzUuWlHI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>