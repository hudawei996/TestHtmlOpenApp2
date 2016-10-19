# TestHtmlOpenApp2 测试使用URL，打开指定的APP。
## 关键一：mainfast文件中，要打开的那个activity，中的intent-filter的配置
## 关键二：HTML文件的配置（如下），放到你的服务器下。让手机的浏览器去访问你配置的这个HTML的地址，既可以吊起指定的APP的activity
###### 代码如下：
情况一：不传递参数
<html>

    <head>

        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
        <title>Insert title here</title>

    </head>

    <body>

        <a href="m://my.com/">打开app</a><br/>

    </body>

</html>
情况二：通过这个方法获取网页带过来的数据
<html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
        <title>Insert title here</title>
    </head>
    <body>
        <a href="m://my.com/?arg0=0&arg1=1">打开app</a><br/>
    </body>
</html>
