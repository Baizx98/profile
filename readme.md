# Profile For Leo
项目地址 https://github.com/Baizx98/profile

## 平台  
### Github
Github是全球最大的免费代码托管平台，使用Git作为版本控制软件。  
我们使用Github来保存源代码和素材，发挥存储服务器的作用。
### Vercel
Vercel可以提供免费的网站托管服务和免费的个性化二级域名。
使用Github账户登陆Vercel，在Vercel中新建项目，并从Github中导入储存个人网站代码和文件的仓库，添加好Custome 域名，以便Vercel接收到来自linhengli.com的请求时，将请求转到本项目 https://zhuanlan.zhihu.com/p/347990778
### GoDaddy
域名提供商，同时提供域名解析服务。
域名解析的作用是当访问linhengli.com时，将访问请求转发到网站托管平台
当使用Vercel托管网站时，需要添加两条解析规则（具体规则参见vercel）  
1. CNAME www cname.vercel-dns.com.
2. A @ 76.76.21.21
## Web
### HTML
### CSS

## 定制
### vscode
vscode是一款轻量级可扩展的代码编辑器，用它编写前端（也就是网页）代码非常方便。  
**必备的插件：**  
- GitLens
- Markdown All in One
- open in browser

### git
在自己的电脑上安装git工具来实现对代码的版本控制

## 开发流程
### 前期准备
1. 在PC上安装vscode和必备插件
2. 在PC上安装git并学习其基本用法(https://www.liaoxuefeng.com/wiki/896043488029600)  
3. 注册github账号
4. 学习github仓库的创建以及如何将自己电脑上的本地代码仓库推送到位于Github的远程仓库 
5. 学习html的基本语法(https://www.runoob.com/html/html-tutorial.html)
6. 学习css的基本语法(https://www.runoob.com/html/html-tutorial.html)

### 部署流程
1. 在本地编写好网页代码
2. 将代码推送至Github
3. 使用Github账户登陆vercel
4. 在vercel中点击Add new，选择project，在Import Git Repository下，选择自己的github账户，并导入储存代码的仓库
5. 进入刚刚创建的project中，点击view domains，在add栏中，输入购买的域名(也就是linhengli.com)，点击configuration可以查看域名的配置规则
6. 登陆GoDaddy，进入域名管理界面中的DNS设置，修改A类型，姓名为@的记录和CNAME类型姓名为www的记录
7. 修改后等待一段时间域名解析生效后就可以正常访问了
8. 后续修改网页代码后只要将最新代码推送到github，vercel会自动更新网站内容，这时访问linhengli.com就可以看到最新的页面

**注意：**vercel会默认将 index.html 作为网站的首页，所以网页主页的文件命名最好为 index.html
