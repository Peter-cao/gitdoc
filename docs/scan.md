# scan
扫码。支持钉钉小程序、微信小程序、微信公众号
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
        <td>type</td>
        <td>钉钉专用， qr：二维码，bar一维码</td>
        <td>string</td>
        <td>否</td>
        <td>qr</td>
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

<h2 id="cid_2">示例</h2>

```html
agileBridge.scan.scanCode({
    type:'qr',//钉钉专用， qr：二维码，bar一维码
    success:function(rs){
        alert(rs)
    },
    fail:function(e){
        console.log(e)
    }
});
```