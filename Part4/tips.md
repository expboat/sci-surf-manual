### **摘要/编码**

场景：论坛讨论留下邮箱，例如[求职帖]()。

#### [**base64**](https://www.v2ex.com/t/482716)

- windows:
```
#TODO
```

- linux:

```
~$ echo "my_email_is_{example[at]email.com base}" | base64
   bXlfZW1haWxfaXNfe2V4YW1wbGVbYXRdZW1haWwuY29tIGJhc2V9Cg==

~$ echo "bXlfZW1haWxfaXNfe2V4YW1wbGVbYXRdZW1haWwuY29tIGJhc2V9Cg==" | base64 --decode 
   my_email_is_{example[at]email.com base}
```

- 搜索引擎

搜索引擎 (如 [duckduckgo](https://www.duckduckgo.com))中查询 "base64 my_email_is_{example[at]email.com base}"  

点击 ![detail](https://github.com/expboat/sci-surf-manual/blob/master/images/part4_details_duckduckgo.png) 中的竖三角查看

<details>
  
![image](https://github.com/expboat/sci-surf-manual/blob/master/images/part4_tips_duckduckgo.png)

</details>

你可以将base64理解为化妆，楼主将邮箱地址'化妆'，网友用卸妆术才能看到邮箱真面目 

~更准确的比喻：邮箱是人，邮箱摘要是这个人的指纹~ 。

这是[v2EX](https://www.v2ex.com)上特有的文化，可能是因为程序员们都喜欢用它来防止爬虫、人肉搜素以及不会化妆的HR，所以在站内流行开来。如果要在其他论坛留下"化妆的邮箱"，最好将本文[链接](https://github.com/expboat/sci-surf-manual/blob/master/Part4/tips.md)附上。

#### hash (md5 sha1 sha256...)
#

[*更详细的解释](/Part4/tips-message-digest.md)
> 预览 摘要与加密 什么是摘要 ...
#
