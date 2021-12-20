# react

#### 接口请求

```js
const request = () => {
  axios
    .get('http://47.96.125.185/api/complete_machine_physical_inventory?page=1&page_size=10&phone=&parts_no=1')
    .then((res) => {
      //console.log(JSON.stringify(res.data));
      console.log(res, '222222');
    })
    .catch((error) => {
      console.log(error);
    });
};
```

##### 类型“AxiosResponse<any, any>”上不存在属性“result”。

![image-20211125145547201](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20211125145547201.png)

解决方法

![image-20211125145630103](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20211125145630103.png)



```

```

