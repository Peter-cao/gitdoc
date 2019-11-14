# button
按钮
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
        <td>text</td>
        <td>显示文本</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>size</td>
        <td>按钮的大小</td>
        <td>string</td>
        <td>default|mini</td>
        <td>default</td>
    </tr>
    <tr>
        <td>type</td>
        <td>按钮的样式类型</td>
        <td>string</td>
        <td>primary|default|warn</td>
        <td>default</td>
    </tr>
    <tr>
        <td>plain</td>
        <td>按钮是否镂空，背景色透明</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>disabled</td>
        <td>是否禁用</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>loading</td>
        <td>名称前是否带 loading 图标</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>hoverClass</td>
        <td>指定按下去的样式类。当 hoverClass="none" 时，没有点击态效果</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>hoverStopPropagation</td>
        <td>指定是否阻止本节点的祖先节点出现点击态</td>
        <td>boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>hoverStartTime</td>
        <td>按住后多久出现点击态，单位毫秒</td>
        <td>Number</td>
        <td>-</td>
        <td>50</td>
    </tr>
    <tr>
        <td>hoverStayTime</td>
        <td>手指松开后点击态保留时间，单位毫秒</td>
        <td>Number</td>
        <td>-</td>
        <td>400</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-button type="primary" text="登录" v-bind:loading="isLogin" v-on:tap="doLogin"></axi-button>
```