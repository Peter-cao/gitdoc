# switch
开关选择器。
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
        <td>disabled</td>
        <td>是否禁用</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>color</td>
        <td>switch 的颜色，同 css 的 color</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
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
        <td>checked 改变时触发 change 事件</td>
        <td>event.detail={ value:checked}</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-switch class="flex-1" id="timing" v-model:switch="formData.detail.timing"></axi-switch>
```