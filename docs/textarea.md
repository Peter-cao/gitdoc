# textarea
多行输入框。
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
        <td>输入框的初始内容</td>
        <td>String</td>
        <td>-</td>
        <td></td>
    </tr>
    <tr>
        <td>placeholder</td>
        <td>输入框为空时占位符</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>placeholderColor</td>
        <td>输入框为空时占位符文字颜色，自定义独有</td>
        <td>String</td>
        <td>-</td>
        <td>#aaaaaa</td>
    </tr>
    <tr>
        <td>disabled</td>
        <td>是否禁用</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>maxlength</td>
        <td>最大输入长度，设置为 -1 的时候不限制最大长度</td>
        <td>Number</td>
        <td>-</td>
        <td>140</td>
    </tr>
    <tr>
        <td>autoHeight</td>
        <td>是否自动增高，设置auto-height时，style.height不生效</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>focus</td>
        <td>是否获取焦点</td>
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
        <td>input</td>
        <td>键盘输入时触发</td>
        <td>event.detail = { value }</td>
    </tr>
    <tr>
        <td>focus</td>
        <td>输入框聚焦时触发</td>
        <td></td>
    </tr>
    <tr>
        <td>blur</td>
        <td>输入框失去焦点时触发</td>
        <td>event.detail = {value: value}</td>
    </tr>
    <tr>
        <td>confirm</td>
        <td>点击完成按钮时触发</td>
        <td>event.detail = {value: value}</td>
    </tr>
    <tr>
        <td>linechange</td>
        <td>输入框行数变化时调用</td>
        <td>event.detail = {height: 0}</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-textarea   v-model:text="formData.detail.title"/>
```