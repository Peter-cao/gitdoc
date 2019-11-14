# store 
缓存。
<h2 id="cid_2">示例</h2>

```html
//设置缓存
agileBridge.store.local("local",this.data.text);
//读取缓存
let result = agileBridge.store.local("local");
//删除缓存
agileBridge.store.removeLocal("local");
```