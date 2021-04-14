# PHPCodeAuditCheckList
 PHP代码审计检查列表

网络收集+自己常见

## 组合拳or常见场景

```
数据库功能模块文件包含+sqlquery读文件造成sql注入

序列化字符串传入点可控，pop链利用

控制器未加auth，未授权访问，关注upload、down、sql

ssrf组合拳

ssrf 

```

## SQL注入

```
magic_quotes_gpc
addslashes
mysql_real_escape_string
intval
```

## XSS

```
print
print_r
echo
printf
sprintf’
die
var_dump
var_export
```

## 文件包含

```
include
include_once
require
require_once
```

## 文件读取

```
file_get_contents
highlight_file
fopen
readfile
fread
fgets
fgetss
parse_ini_file
show_source
file
```
## ssrf

```
curl_setopt
file_get_contents
fsockopen
```

## 文件上传

```
move_upload_file
```

## 代码执行

```
eval
assert
preg_replace
call_user_func
call_user_func_array
array_map
```

## 命令执行

```
system
exec
shell_exec
passthru
pcntl_exec
popen
proc_open
```

## 变量覆盖

```
extract
parse_str
import_request_variables
$$

```

## mysql报错注入

```
floor
updatexml
extracvalue
GeometryCollection
polygon
multipoint
multilinestring
multipolygon
linestring
exp
```

## php安全编码


```
addslashes
mysql_real_escape_string
mysql_escape_string
str_replace
strpos
htmlspecialchars
strip_tags
```

## 防止命令注入

```
escapeshellcmd

escapeshellarg
```