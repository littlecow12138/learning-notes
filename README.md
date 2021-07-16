# learning-notes
# dns修改
可以手动改hosts文件：win 10系统，打开powershell，输入cd \Windows\System32\drivers\etc，切换到hosts文件的路径，然后输入notepad hosts，用记事本打开hosts文件，在最后面加上一行，185.199.110.153 lian-yue.github.io，前面的数字是github.io的IP地址，github.io的IP地址可以在这个网站上查：https://www.ipaddress.com/，有四个我随便选了一个，然后保存文件，然后在powershell输入 Clear-DnsClientCache，清除DNS缓存，然后你再上https://lian-yue.github.io/vue-upload-component/应该就可以了。其他xxx.github.io也是同理，可惜hosts文件不支持通配符，所以只能手动一个一个去改，有点麻烦
