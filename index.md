## 欢迎来到徐某人的独立网站


You can use the [editor on GitHub](https://github.com/xqiiii/xqiiii.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
<h1>666666<h1>
Web开发中的四个域对象：

有范围小到大：page(jsp有效) request(一次请求)session(一次会话) application(当前web应用)

page域指的是pageContext.

request域指的是HttpServletRequest

session 域指的是 HTTPSession

application 域指的是 ServletContext

追所以他们是域对象，原因就是他们都内置了map集合，都有setAttribute getAttribute方法。

他们都有自己固定的生命周期和作用域。

这4个对象的生命周期

声明周期就是值对象的创建到销毁的期间。

page：jsp页面被执行，生命周期开始，jsp页面执行完毕，声明周期结束

request:用户发送一个请求，开始，服务器返回响应，请求结束，生命周期结束

session:用户打开浏览器访问，创建session(开始),session超时或被声明失效，该对象生命周期结束

application：web应用加载的时候创建。Web应用被移除或服务器关闭，对象销毁。[结束]。

Page只在当前jsp有效，每次请求风别对应不同的request.

Request,只在当前请求有效，每次请求分别对应不同的request域

Session只在一次会话中有效，会话结束就无法取到数据了。

四个域对象在选择的时候，能用范围小的绝不用范围大的

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/xqiiii/xqiiii.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
