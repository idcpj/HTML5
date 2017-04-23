# HTML5
响应式的html5网页教程

---

##文件
1.main.css存放都需要应用的样式

2.normailze.css存放个性化的样式，如果个性化的样式过多,可以用html对应的名称创建，如login.css    

####如果项目庞大,采用如下布局
    src
        ├home
            ├css
            ├js
            ├img
        ├login
            ├css
            ├js
            ├img
        ├common
            ├css
            ├js
            ├img
        ├compoent  
            ├alert
            ├layui
            ├uploadify
3.humans.txt
介绍开发者和网站的信息[关于humans.txt链接](http://humanstxt.org/ZH)

4.editorconfig
编辑器格式化时,会先按照该设置
phpstrom需要下载同名插件,使用规则[点击跳转](http://editorconfig.org/)

5.gitignore
让git忽略某些不需要的文件上传到git上

6.强制使用最新的ie进行渲染

    <meta http-equiv="x-ua-compatible" content="ie=edge">
    
7.提醒浏览器更新   
      
    <!--[if lte IE8]>
    <p class="browserupgrade">您的浏览器版本过低,请使用最新版,以获取最佳的体验 <a href="https://browsehappy.com/?locale=zh">升级浏览器</a></p>
    <![endif]-->

8.HTML5标签

    <header>  
    <nav>       导航
    <footer> 
    <article>   文章等独立于页面的内容
    <section>   形成相同内容的区块,<article>为特殊的setcion
    <em>        表示强调
    
9.网页大纲

通过phpstrom 的Structrue 功能来看网页大纲,把section没有标题的变为div

10.normalize.css

相比于传统的css.reset,改css有诸多优势,详情查看连接[链接](http://necolas.github.io/normalize.css/)
来取消不同浏览器之间的差异
   
11.在main.css中设置基础样式

    
    html{
        font-szie:62.5%
        color:#222
    }


>`font-size`设置为62.5%,有利于使用em,他会寻找父元素或祖父元素,都为发现则使用默认`16px=1em`

>rem 参考html的根元素,参考系固定,若html根元素没有设置`font-szie`
,则默认`16px=1rem  `  rem不支持**IE8**

12.li+li
    
    header .top ul li+li{
        border-left: 1px solid #999;
        margin-left: -3px;
    }
    
+表示紧接在li后的所有li,加左边线
margin-left:`<li>`之间的便签会有回车,产生空白符号

13.浮动效果使用

能用`display:inline-bloack` 就不用float,浮动清理困难
