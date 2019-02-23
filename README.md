# vue-elementUI
a background management system(use vue, vue-cli, axios . . . )

### 安装vue-cli 3 
1.卸载vue-cli 2 `npm uninstall vue-cli -g`
2.安装vue-cli 3 `npm install -g @vue/cli`
3.检查版本 `vue --version`
4.创建项目 `vue create hello-world`

### 登录页面
1.安装element-UI,并导入
2.登录页面样式
3.登录功能,axios发送请求,登录状态保存
    + 用v-model双向数据绑定用户名和密码
    + 在main.js中导入axios,配置为Vue.protype.$http
    + .post().then().catch()发送数据,验证登录
    + 登录结果用$message展示
    + 登录成功,用token存储登录状态在localstorge之中

### 中心页面
1.页面样式
2.获取数据,渲染表格

### 优化
1.导航卫士,对未登录者,进行拦截
    + 在main.js中配置全局导航卫士
    + 在页面路由改变时,检测token
    + 有token时,正确跳转
    + 没有时,跳转到登录页