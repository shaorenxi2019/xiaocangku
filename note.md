###1.同源策略
````javascript
//协议  IP地址  端口  都一样就叫同源策略

//同源策略
//http://127.0.0.1:8000/queryInfo
//http://127.0.0.1:8000/A.html


//http://27.0.0.1:63342/5.6/%E4%BB%A3%E7%A0%81/2.%E5%90%8C%E6%BA%90%E7%AD%96%E7%95%A5/static/A.html?_ijt=9b3iilfk4eld8k0fi290kgaqj

````

###非同源
####跨域
**`JSONP跨域`**
>利用script标签的src进行跨域
>1.创建一个script标签
>2.url地址放到src当中
>3.我们需要在url地址最后拼接一个回调函数=函数名
>4.设置全局函数  的函数名就是上边那个函数名


*`cors`*
````javascript
/*
* 1. jsonp （常用）
  2. cors  （常用）
  3. window.name
  4. document.domain  （特定场景）
  5. postMessage (H5)
  6. webpack proxy （webScoket） （常用）
  7. ngix反向代理*/   
  
  
  //在服务器端设置
  //所有端口都可以进行访问
  	// res.header("Access-Control-Allow-Origin", "*");
  	
  	//指定端口进行
  	//res.header("Access-Control-Allow-Origin", "http://127.0.0.1:8000");
````




