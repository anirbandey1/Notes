# Coc-clang setup

```
sudo apt install clang
clang -v
```
To check the version of clangd compiler

You will find a version of g++ , gcc
say version 12

install that version of gcc/g++

```
sudo apt install g++-n
```
where 'n' is the version of g++ to be installed

https://gatowololo.github.io/blog/clangmissingheaders/

https://stackoverflow.com/questions/26333823/clang-doesnt-see-basic-headers


To set code formatting

To reset defaults 
```
cp ~/.clang-format ~/.clang-format-backup
rm ~/.clang-format
```

To get the current clang-format being used
```
clang-format -dump-config <filename.cpp>
```

To copy defaults Replace 
```
clang-format -dump-config <filename.cpp>  > ~/.clang-format
```

In my Arch 
I just set 
to get desired indentation
```
IndentWidth:     4
ObjCBlockIndentWidth: 4
```


