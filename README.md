# sendEmail
*just send some attachments*
> email = Email('12345678@qq.com','password')  
> email.send({'receiver':'receiver@xx.com','attachment':[path1,path2,...]})  

*send a complete email*
> dic = {}  
> dic['subject'] = 'subject'	#default blank	  
> dic['content'] = 'content'	#default blank  
> dic['attachment'] = ['picture.png','readme.txt','sendEmail.py'] #default blank  
> dic['receiver'] = '1799853523@qq.com'  
> sender='12345678@qq.com'      
> password = 'abcdefg'      
> email = Email(sender,password)  

* if you want to conceal your information
> email = Email(sender,password,conceal = True)  