## XCode创建工程后如何不使用`SceneDelegate`
### 一、Xcode11后创建工程会默认创建`SceneDelegate`
![image](https://user-images.githubusercontent.com/70840468/118385069-6560c380-b63e-11eb-91ab-8db7884e8518.png)
### 二、不使用`SceneDelegate`，回到旧的使用`Delegate`的方式
#### 需进行操作如下:
#### 1、删除`SceneDelegate.h`和`SceneDelegate.m`文件
![image](https://user-images.githubusercontent.com/70840468/118385136-03ed2480-b63f-11eb-923e-d374972877c3.png)
#### 2、打开`info.plist`文件，删除key`Application Scene Manifest`
![image](https://user-images.githubusercontent.com/70840468/118385150-254e1080-b63f-11eb-825d-e6d7a3ae40fd.png)
#### 3、打开`AppDelegate.h`文件，添加`window`属性
![image](https://user-images.githubusercontent.com/70840468/118385201-8d045b80-b63f-11eb-965f-322eb9da5ae3.png)

#### 4、打开`AppDelegate.m`文件,删除不需要用到的`UISceneSession lifecycle`代理方法
![image](https://user-images.githubusercontent.com/70840468/118385225-cb9a1600-b63f-11eb-848c-6e1c54b9729d.png)

#### 5、接下来可以开始以往熟悉的操作啦~~~
![image](https://user-images.githubusercontent.com/70840468/118385273-3ba89c00-b640-11eb-8d14-7c20218fd5e7.png)
