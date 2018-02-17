## skia_full (sources sync date was 2018/02/08)
### Project Info
> clone to ***https://skia.googlesource.com/skia.git*** and add google ***depot_tools*** to this project.
### How to use
> clone this project.
```
$ mkdir skia
$ git clone https://github.com/1934016928/skia_full.git
$ cat skia_source.tar.gz* > skia.tar.gz
# rm -rf skia_source.tar.gz*
```
> unzip the tar.gz package.
```
$ tar -zxvf skia.tar.gz
```
> set ***depot_tools*** to system path.
```
$ export PATH=$PATH:${your created skia directory path}/skia/files/depot_tools
```
> test build tools.
```
$ ninja
```
> if tips your ***not found command "ninja"*** or ***"ninja" was not installed***, please check your ***depot_tools*** path and set ***depot_tools*** to system path try agin.
### Config your build.
```
$ bin/gn gen out/Static --args='is_official_build=true'

$ bin/gn gen out/Shared --args='is_official_build=true is_component_build=true'
```
> if you want learn more, please go to ***https://skia.org/*** or click there: ***https://www.jianshu.com/p/f304dd765eb0/***
