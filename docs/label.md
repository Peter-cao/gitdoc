# label
用来改进表单组件的可用性。
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
        <td>for</td>
        <td>绑定控件的 id</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-label for="wx">
    <axi-checkbox id="wx" v-model:checkbox="formData.detail.share" value="1"></axi-checkbox>
    <text class="pr6">微信</text>
</axi-label>
```