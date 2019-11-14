# select
选择框。
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
        <td>placeholder</td>
        <td>没有值的时候的提示语</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>value</td>
        <td>设置为options中某个选项的value值，并且为选中状态</td>
        <td>string</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>options</td>
        <td>select的选项，为对象数组，对象必须包含text和value，为自有属性</td>
        <td>array</td>
        <td>-</td>
        <td>[]</td>
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
        <td>click</td>
        <td>点击事件</td>
        <td></td>
    </tr>
    <tr>
        <td>change</td>
        <td>value 改变时触发 change 事件</td>
        <td>event.detail = {value: value}</td>
    </tr>
</table>
<h2 id="cid_2">示例</h2>

```html
<view class="text-wrapper">
    <text class="text-description">Vertical Scroll 纵向滚动</text>
</view>
<axi-scroll-view class="scroll-block-wrapper">
    <view>
        <view class="bg-green scroll-block-v center">
            <text>A</text>
        </view>
        <view class="bg-blue scroll-block-v center">
            <text>B</text>
        </view>
        <view class="bg-gray scroll-block-v center">
            <text>C</text>
        </view>
    </view>
</axi-scroll-view>

<view class="text-wrapper">
    <text class="text-description">Horizontal Scroll 横向滚动</text>
</view>
<axi-scroll-view direction="horizontal" class="scroll-block-wrapper">
    <view style="flex-direction: row;overflow: auto;">
        <view class="bg-green scroll-block-h center">
            <text>A</text>
        </view>
        <view class="bg-blue scroll-block-h center">
            <text>B</text>
        </view>
        <view class="bg-gray scroll-block-h center">
            <text>C</text>
        </view>
    </view>
</axi-scroll-view>
```
