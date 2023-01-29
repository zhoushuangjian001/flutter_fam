

![icon.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/1277c95cd18843a483fafe8c364a694f~tplv-k3u1fbpfcp-watermark.image?)    
![Author](https://github.com/zhoushuangjian001/flutter-fam/blob/master/images/author.png?raw=true) ![Version](https://github.com/zhoushuangjian001/flutter-fam/blob/master/images/version.png?raw=true&width=30%)![Star](https://github.com/zhoushuangjian001/flutter-fam/blob/master/images/star.png?raw=true)  ![Star](https://github.com/zhoushuangjian001/flutter-fam/blob/master/images/fork.png?raw=true)  


Language: [🇺🇸 English](https://pub.dev/packages/fam) | [🇨🇳 Chinese](https://github.com/zhoushuangjian001/pub_images/blob/master/fam/md/README.md)
## 特别提示
**Fam** 版本的更新方法如下:    
1. **Fam** 版本小于**1.0.5** 的用户使用 `flutter pub global activate fam` 指令升级。
2. **Fam** 版本大于等于 **1.0.5** 的用户使用 `fam --update` 或者 `fam --update x.x.x` 或者 `flutter pub global activate fam` 进行更新。
 
## 一、简述
目前针对 **Flutter**  项目的资产管理服务的工作，**Flutter** 官方建议使用的开发工具（*IDE*）也提供了相应的插件来处理该功能；还有一些大神级别的开发者手写**脚本**或者利用 **Dart** 的自动生成功能写出的管理服务的软件。作为**Flutter** 开发者也好几年了，目前我认为最好的项目资产管服务是**Fam**。

## 二、[Fam](https://pub.dev/packages/fam) 服务
#### 1. Fam 简介
**Fam** 是针对 **Flutter** 项目资产管理服务的**Dart** 脚本服务，它依托于 [pub.dev](https://pub.dev/https://pub.dev/) 平台进行版本控制的。它支持多种平台、操作简单、界面美观、使用便捷等特点。

#### 2. Fam 展示
1. **Fam** 服务下的资产管理文件

    ![fam.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/e50cdf004d25459ba8c6ac1335fa9e77~tplv-k3u1fbpfcp-watermark.image?)
      
     从上图可以看到，**Fam** 将资产文件按目录进行划分，使得项目资产文件所在位置清晰明了，便于查找。
2. **Fam** 服务下的 *pubspec.yaml* 文件配置
                 
    ![fam_pub.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/2ce95a8823b64c6e99e091efd72992ed~tplv-k3u1fbpfcp-watermark.image?)
    
    从上图可以看到，**Fam** 在 *pubspec.yaml* 文件中只进行资产文件目录路径的配置，避免了大片的资产文件的绝对路径的配置。
    
3. **Fam** 服务下的资产使用

    ![fam_use.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/72d4580f3af54fd7b8994951ec730d8b~tplv-k3u1fbpfcp-watermark.image?)
    
    从上图可以看到，**Fam** 使用资产管理类名和点语法来获取资产文件，这使得在项目中使用资产文件更加的便捷。
    
4. **Fam** 服务下的资产使用提示

    ![fam_tiip.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/53c6e5f6721f4db78c1299a2c45339e0~tplv-k3u1fbpfcp-watermark.image?)
    
     从上图可以看到，**Fam** 在使用资产管理文件时，开发编辑器的提示可以完全看全，而不是一些插件的提示都看不全，导致最后选择的也不一定是自己想要的资产文件。


总结: 从上面可以看到 **Fam** 的一些基础展示，同时我相信开发者们此时心里对于各种资产管理的插件或者脚本也有个认识和评估。

## 三、Fam 的配置

**Fam** 是基于 [pub.dev](https://pub.dev/packages/fam) 进行版本管理的。所以可以使用下面指令进行**Fam** 配置。 指令如下:    
`flutter pub global activate fam `。 如果你从来没有全局配置过 **.pub-cache** 的路径，则上面的指令运行后会提示配置 **.pub-cache/bin** 的路径，各个系统提示如下:

1. MacOS 用户
    ![pub-catch.png](https://p9-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/f774c0cf80364a8a8b5e7ee86136570c~tplv-k3u1fbpfcp-watermark.image?)
2. Windows 用户
    ![WechatIMG33.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/99e032546a3b45669b14eb1e5b1ab8fb~tplv-k3u1fbpfcp-watermark.image?)
$\color{#ff0ff0}{📢 注意:}$    
**Windows** 用户由于系统的差异建议使用 `dart pub global activate fam` 指令安装 **fam** 。因为**Window** 系统中当删除 **flutter** 文件使用其他的管理工具时 **pub-cache\bin** 路径也被删除。而 `dart pub global activate fam` 指令生成的 **Pub\Cache\bin** 路径不会被删除。 

按上面提示配置好 **.pub-cache/bin** 路径后，在终端输入执行 `fam help` 或者 `fam -h` 即可检查**Fam** 是否安装成功。 **Fam** 安装成功展示如下:

![fam_help.png](https://p9-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/ffdcf3880e874549866bcf9db86b4069~tplv-k3u1fbpfcp-watermark.image?)

如果  **Fam** 安装失败会提示 `zsh: command not found: fam`。


##  四、 Fam 使用
**Fam** 资产管理服务脚本提供了许多指令，下面我们一一介绍。
1. `fam init`  & `fam -i`  
    作用: 进行 **Flutter** 项目资产管理 **Fam** 服务的初始配置。    
    交互: 该指令执行后，
    1. 让你输入项目资产管理的文件名，默认 **fam.dart** 。
    2. 让你输入项目资产管理的类名，默认 **FamManager** 。 
               
    > 注意:    
        1. 文件名的命名规则是由小写字母和下划线组成且首字母不能是下划线，例如 fam 、 fam_file、 fam_name_file 等。           
        2. 类名的命名规则是由大写字母和小写字母以及下划线组成且首字母必须是大写字母，例如 Fam 、FamManager 、 Fam_Name 等
   
   效果: 指令执行效果
   
    ![fam_init.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/4807eb71527a4d5189c95447d01b716a~tplv-k3u1fbpfcp-watermark.image?)


2. `fam run` & `fam -r`
     
    作用: 有新的资源文件加入项目中时，使用该执行令进行新加资产的管理服务。    
    效果: 执行效果
    
    ![fam_run.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/009f4b7885fe487d818062ae3aa32ce1~tplv-k3u1fbpfcp-watermark.image?)
    
3. `fam fix` & `fam -fi`    

    作用: 修复项目的 **Fam** 配置服务，比如:**Fam** 的资产管理文件被误删除或者 **Fam** 记录文件被误删除等。
    效果: 指令执行效果
    
    ![fam_fix.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/d24448759f924496bca31c36ee0a99bc~tplv-k3u1fbpfcp-watermark.image?)
    
4. `fam filter size`
    
    作用: 检查项目中所有资产文件是否有超过指定大小，默认为  200KB。     
    效果: 默认大小指令 200KB
    
    ![fam_filter_200.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/49d9298532584ef0ab4acc16751856d8~tplv-k3u1fbpfcp-watermark.image?)
    
    效果: 指定大小 10 B
    
    ![fam_filter_b.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/1c85267b68a245709352ab526bb1561a~tplv-k3u1fbpfcp-watermark.image?)
    可以使用  `fam filter size -h` 指令获取帮助，如下:
    
    ![fam_filter_size_h.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/70c46f10361d4051af5d841a3e7aacac~tplv-k3u1fbpfcp-watermark.image?)
    可以使用 `fam filter size -b 10` 或者 `fam filter size -k 10` 或者 `fam filter size -m 10` 或者 `fam filter size -g 10` 等。
    
 
 5. `fam filter unused`
      
    作用: 检查项目中未使用的资产文件。       
    效果: 指令执行效果
    
    ![fam_filyer_unused.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/a5c5f4cb82494710908bf2b1d63b8503~tplv-k3u1fbpfcp-watermark.image?)
    
 6. `fam filter unused --delete` & `fam filter unused -d`
 
    作用: 检查项目中未使用的资产文件同时删除。        
    效果: 指令执行效果
  
      ![fam_filter_unused_d.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9224d181ddc24127b510c65f3b428b1a~tplv-k3u1fbpfcp-watermark.image?)
  
 7.  `fam release` &  `fam version`
 
     作用: 获取 **fam** 线上版本和本地安装版本      
     效果: 指令执行效果
      
      ![fam_v.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/210a203e0f87419c9821ec4f648ae28d~tplv-k3u1fbpfcp-watermark.image?)
      
 8. `fam rename class Assets` 
     
     作用: 重命名**Fam** 服务的资产管理类的类名。      
     效果: 指令执行效果      
     未更改前: 
             
    ![fam_rename_class.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6c4031ff9e4e4f74adb7bf6abd9118c5~tplv-k3u1fbpfcp-watermark.image?)
     更改后管理类变化:
     
    ![fam_rename_class_1.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/927ec5af204442de8f0e8a37d49fc75b~tplv-k3u1fbpfcp-watermark.image?)
    更改后项目使用位置的变化:
    
    ![fam_rename_class_2.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/56bc4d06a69947c5bd9c03c89ef89918~tplv-k3u1fbpfcp-watermark.image?)
 
 9. `fam delete`
     
    **Fam** 的删除服务，我们可以使用 `fam delete  -h` 来查看使用说明:
    
    ![fam_delete.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/1f93cf122aa64c7f939fb88992b97cc4~tplv-k3u1fbpfcp-watermark.image?)
    
    从上面可以知道 `fam delete` 有两个指令，分别是 `fam delete file xx` 单个资产文件删除指令和 `fam delete mfile xx` 多个资产文件删除指令。
    
    删除文件之前:  
    
    ![fam_delete_file_1.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/64a9622a81f24ba3ba66ed60b866b9d9~tplv-k3u1fbpfcp-watermark.image?)
    删除文件之后 : `fam delete file assets/name.webp`
    
    ![fam_delete_flie_2.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/43b163a0fd9542418d23520d50715c7c~tplv-k3u1fbpfcp-watermark.image?)
    
10. `flutter pub global activate fam`
    
    **Fam** 的安装和升级指令。      
    1） 安装看 **Fam 的配置**     
    2） 升级
        
    ![fam_update.png](https://p9-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/8b7feb16618a49ca83ceda3cbd0d63fc~tplv-k3u1fbpfcp-watermark.image?)

## 五、更新 Fam 1.0.5
  1. 新指令添加    
     - **`fam --version`**    
        获取当前安装的 Fam 的版本。
     - **`fam --releases`**    
        获取 Fam 所有可安装的稳定版本。
     - **`fam --update` & `fam --update x.x.x`**    
        Fam 升级到最新版本，也可以指定版本升级。
    
## 六、总结
  以上是 **Fam** 的基础介绍。**Fam** 的 **pub.dev** 地址是 [Fam 地址 ](https://pub.dev/packages/fam) 以及**Git** 地址是 [Fam 地址](https://github.com/zhoushuangjian001/fam)。 欢迎各位大佬点赞和喜欢。
