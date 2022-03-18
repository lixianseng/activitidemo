拷过来的mysql的驱动是5点几，但是我电脑上安装的是8点几点，所有讲version改成8.0.21。navicat的版本也是8.0.21
还是会报错：Caused by: com.mysql.cj.exceptions.CJCommunicationsException: Communications link failure
驱动的连接报错。
把<property name="url" value="jdbc:mysql://lcoalhost:3306/activiti?useUnicode=true" />中的locahost改成127.0.0.1，就成功了。
