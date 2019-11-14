# checkbox
复选框组件
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
        <td>选中时触发checkbox-group的 change 事件，并携带 checkbox 的 value</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>disabled</td>
        <td>是否禁用</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
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

<h2 id="cid_2">示例</h2>

```html
<axi-label for="wx">
    <axi-checkbox id="wx" v-model:checkbox="formData.detail.share" value="1"></axi-checkbox>
    <text class="pr6">微信</text>
</axi-label>
<axi-label for="dd">
    <axi-checkbox id="dd" v-model:checkbox="formData.detail.share" value="2"></axi-checkbox>
    <text class="pr6">钉钉</text>
</axi-label>
<axi-label for="wb">
    <axi-checkbox id="wb" v-model:checkbox="formData.detail.share" value="3"></axi-checkbox>
    <text>微博</text>
</axi-label>
```