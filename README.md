# checkstyle_export_excel
使用 checkstyle 导出 excel


工作需要，开始学习使用checkout，学习过程如下：
1.可以使用 gradle 导出 html
2.使用 checkstyle jar 包，命令行导出 文本/XML 
3.使用 checkstyle 源代码，直接运行，导出 文本/XML，可自定义导出，如 excel

使用 gradle 导出
参考 https://www.cnblogs.com/woshimrf/p/using-checkstyle.html

使用 jar 包导出
参考 https://blog.csdn.net/cyj083/article/details/77044030

使用源码导出
原料：
1.checkstyle-v8.28-https://github.com/checkstyle/checkstyle
2.poi-v4.1.1-https://poi.apache.org
3.poi 写 excel -https://poi.apache.org/components/spreadsheet/quick-guide.html

在 com.puppycrawl.tools.checkstyle.DefaultLogger 类

- auditStarted 输出开始
- addError 输出日志
- addException 输出日志（我没用到）
- auditFinished 输出结束

在 start 方法里初始化 POI 相关
在 add 方法里使用 POI 写具体内容
在 finish 方法里处理结束的内容







