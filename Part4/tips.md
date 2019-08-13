`出入于安全考虑，应尽可能只使用系统自带工具，不使用第三方软件、在线网站查询`

#

### **1 摘要/编码**



#### [**base64编码与解码**](https://www.v2ex.com/t/482716)

场景：论坛讨论留下编码后的邮箱

#

- windows:

在 D:\ 创建文本文件 file.txt ，内容如下：

`my_email_is_{example[at]email.com base}`

Windows 徽标键 ![win-icon-WindowsLogo](https://github.com/expboat/sci-surf-manual/blob/master/images/win-icon-WindowsLogo.png) + R (打开“运行”对话框)

“运行”对话框中输入：

 `powershell`
 
powershell 中输入：

```
cd D:\

CertUtil -encode file.txt encode.txt
CertUtil -decode encode.txt decode.txt 
```

其中，base64 编码就在 encode.txt 中。

#

- linux:

```
~$ echo "my_email_is_{example[at]email.com}" | base64
   bXlfZW1haWxfaXNfe2V4YW1wbGVbYXRdZW1haWwuY29tfQo=

~$ echo "bXlfZW1haWxfaXNfe2V4YW1wbGVbYXRdZW1haWwuY29tfQo=" | base64 --decode 
   my_email_is_{example[at]email.com}
```

#

- 搜索引擎

搜索引擎 (如 [duckduckgo](https://www.duckduckgo.com))中查询 "base64 my_email_is_{example[at]email.com base}"  

点击 ![detail](https://github.com/expboat/sci-surf-manual/blob/master/images/part4_details_duckduckgo.png) 中的竖三角查看

<details>
  
![image](https://github.com/expboat/sci-surf-manual/blob/master/images/part4_tips_duckduckgo.png)

</details>

#



这是[v2EX](https://www.v2ex.com)特有的文化，可能是因为程序员们都喜欢用它来防止爬虫、人肉搜素以及不会化妆的HR所以在站内流行开来。


#

#### hash (md5 sha1 sha256...)

#

[*更详细的解释](/Part4/tips-message-digest.md)
> 预览 摘要与加密 什么是摘要 ...
#


[其他windows下快捷方式](https://support.microsoft.com/zh-cn/help/12445/windows-keyboard-shortcuts)
