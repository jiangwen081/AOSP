Android在C/C++封装了许多好用的API，记录一下，方便阅读

### 1.android::base::Split 
分割字符串，用法
```C
std::vector<std::string> pieces = android::base::Split(entry, "=");
        if (pieces.size() == 2) {
            fn(pieces[0], pieces[1], in_qemu);
        } 
```
### 2.android::base::ReadFdToString(int fd, std::string* content ) 
读取文件内容到字符串,fd是文件描述符，content是读取到哪个字符串中
