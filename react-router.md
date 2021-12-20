### **react-router**

###### exact：`exact`默认为false，如果为true时，需要和路由相同时才能匹配，但是如果有斜杠也是可以匹配上的。 如果在父路由中加了`exact`，是不能匹配子路由的,建议在子路由中加`exact`，如下所示

```react
//父路由
<Switch>
    <Route path="/a" component={ComponentA} />
</Switch>

```

```react
//子路由，tuanDetail组件里
<Switch>
        <Route path="/a/b" exact component={ComponentB}/>
</Switch>

```

###### strict：`strict`默认为false，如果为true时，路由后面有斜杠而url中没有斜杠，是不匹配的

![image.png](https://p1-jj.byteimg.com/tos-cn-i-t2oaga2asx/gold-user-assets/2019/5/9/16a9d2eda0ae8843~tplv-t2oaga2asx-watermark.awebp)

总结：如果没有子路由的情况，配路由加一个`exact`；如果有子路由，建议在子路由中加`exact`，父路由不加； 而`strict`是针对是否有斜杠的，一般可以忽略不配置。