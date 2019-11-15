# 页面定义

页面文件以<code>.axp</code>结尾。页面访问路径为src往后的目录结构+文件名。


页面结构如下

```html
<script>
PageWrapper({
    onLoad: function(){
        // 页面加载后触发
    },
    onShow: function(){
        // 页面显示后触发，包括上一页面返回当前页面
    },
    data: {
        // 页面数据
    },
    methods: {
        // 页面的方法列表
    },
    observers: {
        // 监听数据变化
        /*
        形如：
        'key1.key2.key3': function(){
            // 当data中key1.key2.key3值变化时触发
        }
        */
    }
    // 页面方法
});
</script>
<style>
    //样式
</style>
<ui>
    //页面
</ui>
```


# 组件定义

组件文件以<code>.axc</code>结尾。组件无需引用即可使用，组件对应的标签名即为组件文件名，文件名一般为英文小写，单词间以-连接。

组件结构如下：

```html
<script>
ComponentWrapper({
    data: {
        // 组件绑定的数据，仅支持基础数据
    },
    properties: {
        /*
        形如：
        propName: {
            type: String|Object|Boolean|Number,
            value: 默认值，可无,
            observer: Function，可无
        }
        */
    },
    methods: {
        // 组件的方法列表
    },
    observers: {
        // 监听数据变化
    }
});
</script>
<style>
    //样式
</style>
<ui>
    //页面
</ui>

```