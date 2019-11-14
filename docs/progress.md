# progress
进度条。
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
        <td>showInfo</td>
        <td>在进度条右侧显示百分比</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>borderRadius</td>
        <td>圆角大小，单位px</td>
        <td>Number</td>
        <td>-</td>
        <td>0</td>
    </tr>
    <tr>
        <td>fontSize</td>
        <td>右侧百分比字体大小，单位px</td>
        <td>Number</td>
        <td>-</td>
        <td>16</td>
    </tr>
    <tr>
        <td>strokeWidth</td>
        <td>进度条线的宽度，单位px（2.4.0起支持rpx）</td>
        <td>Number</td>
        <td>-</td>
        <td>6</td>
    </tr>
    <tr>
        <td>activeColor</td>
        <td>已选择的进度条的颜色</td>
        <td>string</td>
        <td>-</td>
        <td>#09BB07</td>
    </tr>
    <tr>
        <td>backgroundColor</td>
        <td>未选择的进度条的颜色</td>
        <td>string</td>
        <td>-</td>
        <td>#bebebe</td>
    </tr>
    <tr>
        <td>active</td>
        <td>进度条从左往右的动画</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>activeMode</td>
        <td>backwards: 动画从头播；forwards：动画从上次结束点接着播</td>
        <td>string</td>
        <td>backwards|forwards</td>
        <td>backwards</td>
    </tr>
    <tr>
        <td>percent</td>
        <td>百分比0~100</td>
        <td>Number</td>
        <td>-</td>
        <td>0</td>
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
        <td>activeend</td>
        <td>动画完成事件</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<axi-progress percent="40" v-bind:active="true" activeMode="forwards" borderRadius="5" strokeWidth="10" style="margin-right:20mpx;flex:1;"></axi-progress>
```