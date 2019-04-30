# sendEmail
*make sure your email SMTP is supported and get the code*  
*make sure you have an access to the Internet*  

## Install  
> pip install sendEmail198
> from sendEmail198.sendEmail198 import Email

## Usage
* make a dictionary consisted of the information
> dic = {}  
> dic['subject'] = 'subject'	#default blank	  
> dic['content'] = 'content'	#default blank  
> dic['attachment'] = ['picture.png','readme.txt','sendEmail.py'] #default blank  
> dic['receiver'] = '1799853523@qq.com'  
> sender='12345678@qq.com'      
> password = 'abcdefg'    # the code given by your email server  
> email = Email(sender,password)

* a simple way if you just want to send some files without destription
> email = Email('12345678@qq.com','password')  
> email.send({'receiver':'receiver@xx.com','attachment':[path1,path2,...]})    

* if you want to conceal your information
> email = Email(sender,password,conceal = True)  