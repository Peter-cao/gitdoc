# refresh
下拉刷新组件。

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
<axi-refresh class="scroll-view" v-on:pulldown="pulldown" v-on:pullup="pullup">
    <view class="scroll-wrapper center-h">
        <view class="head-title center">
            <text>{{pageTitle}}</text>
        </view>
        <view class="scroll-view-list">
            <view v-for="item in list" class="scroll-view-item"><text>{{item.title}}</text></view>
        </view>
    </view>
</axi-refresh>
```