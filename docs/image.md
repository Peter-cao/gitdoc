# image
图片。支持JPG、PNG、SVG格式
<h2 id="cid_1">属性</h2>
<table>
    <tr>
        <th>属性</th>
        <th>说明</th>
        <th>类型</th>
        <th>可选值</th>
        <th>默认值</th>
    </tr>
    <tr>
        <td>src</td>
        <td>图片地址</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>mode</td>
        <td>图片裁剪、缩放的模式</td>
        <td>string</td>
        <td>只支持三种小程序的scaleToFill、aspectFill、aspectFit和扩展autoFit</td>
        <td>scaleToFill</td>
    </tr>
    <tr>
        <td>checked</td>
        <td>当前是否选中，可用来设置默认选中</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>color</td>
        <td>checkbox的颜色，同css的color</td>
        <td>string</td>
        <td>-</td>
        <td>#09bb07</td>
    </tr>
</table>

<h2 id="cid_2">事件</h2>

<table>
    <tr>
        <th>事件名</th>
        <th>说明</th>
        <th>参数</th>
    </tr>
    <tr>
        <td>error</td>
        <td>当错误发生时，发布到 AppService 的事件名</td>
        <td>event.detail = {errMsg: 'something wrong'}'</td>
    </tr>
    <tr>
        <td>load</td>
        <td>当图片载入完毕时，发布到 AppService 的事件名</td>
        <td>event.detail = {height:'图片高度px', width:'图片宽度px'}</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-image src="https://www.baidu.com/img/baidu_jgylogo3.gif" mode="autoFit"></axi-image>
<axi-image src="https://www.baidu.com/img/baidu_jgylogo3.gif" mode="scaleToFill" style="width:200mpx;height:30mpx;"></axi-image>
<axi-image src="https://www.baidu.com/img/baidu_jgylogo3.gif" mode="aspectFill" style="width:200mpx;height:30mpx;"></axi-image>
<axi-image src="https://www.baidu.com/img/baidu_jgylogo3.gif" mode="aspectFit" style="width:200mpx;height:30mpx;"></axi-image>
</axi-label>
```