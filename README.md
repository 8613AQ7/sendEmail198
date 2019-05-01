# sendEmail
*make sure your email SMTP is supported and get the code*  
*make sure you have an access to the Internet*  

## Install  
> pip install sendEmail198  

## Usage
```python
from sendEmail198.sendEmail198 import Email  
sender='12345678@qq.com'       
password = 'abcdefg'    # the code given by your email server   
email = Email(sender,password)  
```  
* make a dictionary consisted of the information    
```python  
dic = {}   
dic['subject'] = 'subject'	#default blank	  
dic['content'] = 'content'	#default blank  
dic['attachment'] = ['picture.png','readme.txt','sendEmail.py'] #default blank  
dic['receiver'] = '1799853523@qq.com'  
email.send(dic)  
```
* a simple way if you just want to send some files without destription  
```python  
email = Email('12345678@qq.com','password')    
email.send({'receiver':'receiver@xx.com','attachment':[path1,path2,...]})     
```
* if you want to conceal your information
```python
email = Email(sender,password,conceal = True)    
```