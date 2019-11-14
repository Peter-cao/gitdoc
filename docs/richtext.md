# richtext
富文本组件。
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
        <td>selectable</td>
        <td>文本是否可选</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>space</td>
        <td>是否显示连续空格</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>text</td>
        <td>显示的文本，非标</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>nodes</td>
        <td>HTML String</td>
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
        <td>pulldown</td>
        <td>下拉刷新触发</td>
        <td>-</td>
    </tr>
    <tr>
        <td>pullup</td>
        <td>上滑触发</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
 <axi-textarea maxlength="-1" class="rich-text-editor"  v-model:text="htmlSnip"></axi-textarea>
 <!-- 小程序rich-text在组件内部则样式不生效，只有在page内才生效，如果html中使用了样式建议直接使用rich-text -->
 <rich-text v-if="env==='miniprogram'" v-bind:nodes="htmlSnip"></rich-text>
```