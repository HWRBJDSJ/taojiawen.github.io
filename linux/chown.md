# 文件及目录权限管理

## 权限

	 读(r)：读取文件的内容；列出目录里的对象
	 写(w)：允许修改文件；在目录里面新建或者删除文件
	 执行(x)：允许执行文件；允许进入目录里
	
### 数字权限
	
	 读：4
	 写：2
	 执行：1

## chmod命令
	
	格式 
	 chmod [ugoa] [+-=] [rwx] file/dir 或 chmod nnn file/dir
	 
	参数解释
	 u:属主  g:属组  o:其他用户  a:所有用户
	 +:添加权限  -:删除权限  =:赋予权限
	 nnn:三位八进制的权限
	 
	常用命令选项
	 -R 递归修改指定目录下的所有子文件及文件夹的权限
	 -f 强制改变文件访问特权；如果是文件的拥有者，则得  不到任何错误信息
	 
## chown命令

	格式
	 chown 属主 file/dir 
	 chown :属组 file/dir
	 chown 属主:属组 file/dir
	
	常用命令选项
	 -R：递归的修改指定目录下所有文件、子目录的归属