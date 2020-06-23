#### Electron 是 Github 发布跨平台桌面应用开发工具，支持 Web 技术开发桌面应用开发。代表项目有Github的Atom和Microsoft的VSCode。

一般在其文件resources中存在app.asar和electron.asar等.asar后缀的文件。而主要的源码是以打包的形式存放在app.asar中，我们需要将app.asar解包并分析出其关键代码。

### 解app.asar包

#### 1、先安装Nodejs，安装包中自带npm

#### 2、安装asar

```
命令为：npm -g instal asar
```

3、安装好之后，进入需要解压的app.asar的文件中执行命令

用 asar extract 反编译/解压

```
asar extract app.asar ./myapp
```

app.asar是需要解压的文件

./myapp需要解压到的文件夹

asar pack 打包

```
asar pack your-app app.asar
```

