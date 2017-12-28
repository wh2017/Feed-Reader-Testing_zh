## 订阅阅读器测试

### 项目简介

这是一个基于 web 的用来读取 rss 源的应用。在项目中，进行能够全面检测项目（RSS Feed 测试、RSS Feed 属性、菜单默认状态和显示/隐藏菜单）功能的所有必要测试。

### 项目目的

测试是开发过程中一个很重要的部分，很多组织把一个标准的开发过程称之为测试驱动开发。意思就是开发人员在开始着手编写应用代码之前先写好测试用例。当然这个时候所有的测试用例都是通不过的，然后就开始编写应用代码使测试全部通过。

### 项目运行

#### 方法一

1. 将这个代码库导出
2. 你可以运行一个本地服务器

```bash
  $> cd /你的工程目录
  $> python -m SimpleHTTPServer 8080
```
#### 方法二

1. 打开浏览器，访问 localhost:8080
2. 下载 [ngrok](https://ngrok.com/) 并将其安装在你的工程根目录下，让你的本地服务器能够被远程访问。

``` bash
  $> cd /你的工程目录
  $> ./ngrok http 8080
```
#### 方法三

右击index.html文件 => 打开方式 => 选择一款本地安装的浏览器



### 项目步骤

1. 上一下 javascript Testing [课程](https://www.udacity.com/course/ud549)

2. 下载[必要的项目资源](http://github.com/udacity/frontend-nanodegree-feedreader)

3. 在浏览器里面查看一下应用的功能

4. 查看项目的 HTMl (**./index.html**), CSS (**./css/style.css**) 和 JavaScript (**./js/app.js**) 文件来对项目的工作原理有一个基本的了解。

5. 查看 Jasmine spec 文件 **./jasmine/spec/feedreader.js** 然后翻阅阅读 [Jasmine 文档](http://jasmine.github.io)。

6. 编辑 **./js/app.js** 里面的 `allFeeds` 变量使给出的测试通不过，然后观察Jasmine是怎么展示你应用的错误信息的。

7. 将 `allFeeds` 变量返回给一个短暂的状态。（待修改）

8. 编写一个测试遍历 allFeeds 对象里面的所有的源来保证有链接字段而且链接不是空的。

9. 编写一个测试遍历 allFeeds 对象里面的所有的源来保证有名字字段而且不是空的。

10. 写一个叫做 `"The menu"` 的测试用例

11. 写一个测试用例保证菜单元素默认是隐藏的。你需要分析 html 和 css 来搞清楚我们是怎么实现隐藏/展示菜单元素的。

12. 写一个测试用例保证当菜单图标被点击的时候菜单会切换可见状态。这个测试应该包含两个 expectation ： 党点击图标的时候菜单是否显示，再次点击的时候是否隐藏。

13. 写一个叫做 `"Initial Entries"` 的测试用例

14. 写一个测试保证 `loadFeed` 函数被调用而且工作正常，即在 `.feed` 容器元素里面至少有一个 `.entry` 的元素。

15. 写一个叫做 `"New Feed Selection"` 的测试用例

16. 写一个测试保证当用 `loadFeed` 函数加载一个新源的时候内容会真的改变。

17. 每个测试都不应该依赖别的测试的结果。

18. 回调函数应该用来保证在测试运行之前源已经被加载。

19. 实现未定义变量和数组越界的错误处理。

20. 当完成所有任务的时候，所有的测试也应该通过。

