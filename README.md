# ASP.NET-Memshell-Scanner v1.0
 asp.net内存马检测工具，通过aspx脚本来实现asp.net内存马的检测以及查杀。

核心代码来源于：[yzddmr6/As-Exploits](https://github.com/yzddmr6/As-Exploits)

前端样式风格参考：[c0ny1/java-memshell-scanner](https://github.com/c0ny1/java-memshell-scanner)

## 支持类型

* VirtualPath内存马 (蚁剑、哥斯拉)

## 使用

上传aspx-memshell-scanner.aspx到web目录，浏览器访问即可。

### 默认情况

![image-20211219152259442](README.assets/image-20211219152259442.png)

如果业务中不存在添加虚拟目录的代码，默认只会有一条结果。

注意：System.Web.Hosting.MapPathBasedVirtualPathProvider为系统默认VirtualPathProvider，请勿删除，否则会导致网站崩溃。

### 存在内存马的情况

![image-20211219152006471](README.assets/image-20211219152006471.png)

其中类名为memoryShell.GodzillaVirtualPathProvider为哥斯拉的内存马

MemShell.SamplePathProvider为蚁剑的内存马

### 清除内存马

点击kill，提示操作成功，即可删除内存马。

![image-20211219152132513](README.assets/image-20211219152132513.png)

## 更新日志

### v1.0 (2021.12.19)

* release