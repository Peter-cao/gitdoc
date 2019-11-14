# location
定位。
<h2 id="cid_2">参数</h2>
<table>
    <tr>
        <th>参数</th>
        <th>说明</th>
        <th>类型</th>
        <th>必填</th>
        <th>默认值</th>
    </tr>
    <tr>
        <td>success</td>
        <td>接口调用成功的回调函数</td>
        <td>function</td>
        <td>否</td>
        <td>-</td>
    </tr>
    <tr>
        <td>fail</td>
        <td>接口调用失败的回调函数</td>
        <td>function</td>
        <td>否</td>
        <td>-</td>
    </tr>
</table>
<h2 id="cid_2">success 回调函数参数</h2>
<table>
    <tr>
        <th>参数</th>
        <th>说明</th>
        <th>类型</th>
    </tr>
    <tr>
        <td>latitude</td>
        <td>纬度，范围为 -90~90，负数表示南纬</td>
        <td>number</td>
    </tr>
    <tr>
        <td>longitude</td>
        <td>经度，范围为 -180~180，负数表示西经</td>
        <td>number</td>
    </tr>
</table>
<h2 id="cid_2">示例</h2>

```html
agileBridge.location.getLocation({
    success:function(res){
        comp.setData({
            latitude: res.latitude,
            longitude: res.longitude
        });
    },
    error:function(error){
        console.log(error)
    }
})
```
