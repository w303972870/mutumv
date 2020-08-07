# 项目背景：
    因业务需要，有一个目录迁移的需求，属于多层级mv，有接近2亿个文件，使用简单的mv命令无法进行文件移动，所以开发
    一个小工具，进行《从一个源目录移动文件到目标目录》，已经规避两个分区使用了不同的文件系统导致的 invalid cross-device link 错误
    
# 使用说明：
    1. Linux系统：仅仅是使用的话可以只直接下载根目录中的mutumv文件，然后赋予可执行权限，chmod +x mutumv ，最后就可以使用了
    2. Windows系统：仅仅是使用的话可以只直接下载根目录中的mutumv.exe文件，将mutumv.exe放到C:\Windows\System32目录下，
       然后在cmd中直接使用命令mutumv即可
    
    运行命令后会在执行命令的当前目录下形成一个日志，日志会记录详细的操作
    
# 命令说明：
    Usage: mutumv [-from sourcedir] [-to target.dir]
        Options:
            -from string
                源目录，从这个目录移动
            -to string
                目标目录，移动到这个目录下
