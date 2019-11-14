# 路由

<h2 id="cid_2">示例</h2>

```html
//跳转到应用内的某个页面
agileBridge.navigator.navigateTo({
    url: url
});

//关闭当前页面，返回上一页面
agileBridge.navigator.navigateBack();

//关闭当前页面，跳转到应用内的某个页面。
agileBridge.navigator.redirectTo({
    url: 'pages/cms/index'
});
```