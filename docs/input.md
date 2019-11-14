# input
输入框。

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
        <td>blur</td>
        <td>输入框聚焦时触发</td>
        <td>-</td>
    </tr>
    <tr>
        <td>focus</td>
        <td>输入框失去焦点时触发</td>
        <td>event.detail = {value: value}</td>
    </tr>
    <tr>
        <td>confirm</td>
        <td>点击完成按钮时触发</td>
        <td>event.detail = {value: value}</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-input v-model:text="formData.login.username" type="text" placeholder="手机/邮箱"></axi-input>
```