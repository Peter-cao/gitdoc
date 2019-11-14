# view
视图容器。
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
        <td>hoverClass</td>
        <td>指定按下去的样式类。当 hover-class="none" 时，没有点击态效果</td>
        <td>String</td>
        <td>-</td>
        <td></td>
    </tr>
    <tr>
        <td>hoverStopPropagation</td>
        <td>指定是否阻止本节点的祖先节点出现点击态</td>
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
<view class="text-wrapper">
    <text class="text-description">flex-direction: row 横向布局</text>
</view>
<view class="row-wrapper">
    <view class="bg-green row-width">
        <text>A</text>
    </view>
    <view class="bg-blue row-width">
        <text>B</text>
    </view>
    <view class="bg-gray row-width">
        <text>C</text>
    </view>
</view>

<view class="text-wrapper">
    <text class="text-description">flex-direction: column 纵向布局</text>
</view>
<view class="column-wrapper">
    <view class="bg-green column-width">
        <text>A</text>
    </view>
    <view class="bg-blue column-width">
        <text>B</text>
    </view>
    <view class="bg-gray column-width">
        <text>C</text>
    </view>
</view>
```