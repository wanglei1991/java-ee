你会发现spring-webmvc这个pom文件里面有commons-loggings这个jar包【在Maven Dependencies中看到】，
所以此时你只需导入log4j的jar包，并配置log4j.properties文件即可使用log4j记录日志。但是这里没有用。

缓存：
由于一个get得到的结果直接对应到一个URL，所以get的结果页面有可能被浏览器缓存，而post一般不能。
所以当你不改变文本框中的值时，
重复点击profile按钮，只有第一次会将请求提交到服务器。
而重复点击login按钮，每一次都会讲请求提交到服务器。