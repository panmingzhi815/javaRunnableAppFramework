# javaRunnableAppFramework
一个可在windows上直接运行的java桌面应用软件

使用maven package 进行打包后，会在target目录下生成一个文件夹，在文件夹中有一个windows 可运行文件main.exe,还有一个配置文件main.ini 。 在ini配置文件中，可配置程序启动时使用哪个类的main作为入口。

lib目录为maven package时自动拷贝的jar包依赖，这其中也包括本项目最终生成的jar包。

jre为java可运行环境，package 打包时，为自动拷贝本机的jre到些目录下。这样运行main.exe时就不再需要在pc上再安装java虚拟机了。

ini配置文件中包含log = log.txt ，此行定义当前程序默认输出的日志文件，一般来讲程序会自动定义日志输入文件位置。这个配置只是方便程序在不正常启动时方便查找问题。
