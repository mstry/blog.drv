# 1. 安装依赖 #

## 1.1 nodejs包 ##

	Nodejs包依赖在源码文件package.json里，在源码目录下用npm下载依赖

	```bash
	npm install
	```
	
	如果nodejs依赖包下载速度慢，可以从百度云盘下载安装
	
	```bash
	bypy downfile hexo/node_modules-hexo.tar.xz
	tar xJf node_modules-hexo.tar.xz
	```

## 2.1 源码模块 ##

	模块依赖声明在.gitmodules，可以用git命令安装
	
	```bash
	git submodule update --force --init --recursive
	```
	
	```bash
	git submodule update --force --init --recursive source
	git submodule update --force --init --recursive themes/next
	```
	如果themes/next下载速度慢，可以从百度云盘下载安装
	
	```bash
	bypy downfile dot-git-modules-themes-next.tar.xz
	tar xJf dot-git-modules-themes-next.tar.xz -C .git/modules/themes/
	bypy downfile theme-next.tar.xz
	tar xJf theme-next.tar.xz -C themes/
	```
	
# 2. 调试发布 #

- 本地启动
- 发布部署
