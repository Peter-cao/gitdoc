# picktime
时间选择。
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
        <td>value</td>
        <td>默认值</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>end</td>
        <td>最大可选时间</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>start</td>
        <td>最小可选时间</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>placeholder</td>
        <td>占位符</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>disabled</td>
        <td>是否禁用</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
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
        <td>change</td>
        <td>value 改变时触发 change 事件</td>
        <td>event.detail = {value: value}</td>
    </tr>
    <tr>
        <td>cancel</td>
        <td>取消选择时触发</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-pick-time class="flex-1" v-model:select="formData.detail.sendDate" placeholder="请选择发送日期"></axi-pick-time>
```