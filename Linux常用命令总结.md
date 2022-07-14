# 基本常用命令

##  复制剪切删除命令

###  复制命令：cp
复制文件
```shell
cp 要复制的文件 目标目录
```
复制目录

```shell
cp -r 要复制的目录 目标目录
```

### 剪切命令：mv

剪切文件
```shell
mv 要复制的文件 目标目录
```
剪切目录

```shell
mv 要复制的目录 目标目录
```

### 删除命令：rm

删除文件和目录

```shell
rm -rf alphapose
```

##  压缩与解压缩命令
### .zip格式

基本格式




### .tar.gz格式
将“qzm2210”和“qzm2205”两个文件夹合并压缩为qzm.tar.gz
```shell
tar -zcvf qzm.tar.gz /qzm2110 /qzm2205
```
解压缩qzm.tar.gz
```shell
tar -zxvf qzm.tar.gz
```

## 关机与重启

### 关机

```shell
poweroff
```

### 重启
```
reboot
```
# 文件系统相关

## 文件系统查看命令：df

基本格式
```shell
df [选项] [挂载点或设备分区文件名]
```

查看所有已挂载文件系统的信息

```shell
df -h
```

## 统计目录或文件所占磁盘空间大小命令：du
基本格式

```
du [选项] [目录或文件名]
```

查看当前文件夹下下一级子目录大小

```shell
du -h --max-depth=1
```
查看当前目录所占磁盘空间的大小

```shell
du -sh
```

# Linux命令杂项

## 多条命令同时执行语法

不管前一个命令运行成功还是出现错误，只要其运行结束，后一个都会在它之后运行

```text
cmd1; cmd2; cmd3
```

只有在前一个命令成功运行结束时，下一个命令才会运行

```text
cmd1 && cmd2 && cmd3
```

只有在前一个命令出现错误时，才运行下一个命令

```text
cmd1 || cmd2 || cmd3
```