## Information

```c
Exploit Title:JSPGOU v6.0-Cross Site Scripting(XSS)
Exploit date:02.06.2021
Exploit Author:Al1ex@Heptagram
Vendor Homepage:https://www.jeecms.com/
Affect Version:JSPGOU v6.0
Description:There is an XSS vulnerability in jspgou foreground commodity consultation function module. The attacker can steal the cookie information of any user through this vulnerability.
```

## How to Exploit

Step  1：register a user and login in

![img](img/1.png)

Step 2：Select any product and enter the introduction page

![img](img/2.png)

Step 3：insert malicious XSS code at the commodity consultation

```
2<img src=x onerror=alert(/xss/);>
```

![img](img/3.png)

When other users view product information, malicious XSS can be triggered successfully

![img](img/4.png)

## Reference

https://www.jeecms.com/

