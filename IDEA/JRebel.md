# `JRebel`

> Restart vs Reload
>
> The restart technology provided by Spring Boot works by using two classloaders. Classes that do not change (for example, those from third-party jars) are loaded into a *base* classloader. Classes that you are actively developing are loaded into a *restart* classloader. When the application is restarted, the *restart* classloader is thrown away and a new one is created. This approach means that application restarts are typically much faster than “cold starts”, since the *base* classloader is already available and populated.
>
> If you find that restarts are not quick enough for your applications or you encounter classloading issues, you could consider reloading technologies such as [JRebel](https://jrebel.com/software/jrebel/) from ZeroTurnaround. These work by rewriting classes as they are loaded to make them more amenable to reloading.

`IDEA`中如何使用`JRebel`

- [获取`GUID`](https://www.guidgen.com/)

- 将生成好的`GUID` 字符串拼接到网址：`https://jrebel.qekang.com/`

  ```https
  https://jrebel.qekang.com/cb8888bb-9d43-4115-bf4b-10539349cf2d
  ```

- 打开 `JRebel` 的面板，在` Connect to online licensing service `一栏输入你的激活地址和邮箱

- 离线模式，来防止失效，`File -> Settings -> JRebel -> [Work offline]`按钮。

