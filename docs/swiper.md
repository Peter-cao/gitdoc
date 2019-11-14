# swiper
滑块视图容器。
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
        <td>type</td>
        <td>slider显示模式,bridge属性，当为gallery时对应wx小程序的previous-margin和next-margin</td>
        <td>String</td>
        <td>normal|zoom|depth|gallery</td>
        <td>normal</td>
    </tr>
    <tr>
        <td>vertical</td>
        <td>滑动方向是否为纵向</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>autoplay</td>
        <td>是否自动切换</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>interval</td>
        <td>自动切换时间间隔</td>
        <td>Number</td>
        <td>-</td>
        <td>5000</td>
    </tr>
    <tr>
        <td>interval</td>
        <td>自动切换时间间隔</td>
        <td>Number</td>
        <td>-</td>
        <td>5000</td>
    </tr>
    <tr>
        <td>current</td>
        <td>当前所在滑块的 index</td>
        <td>Number</td>
        <td>-</td>
        <td>0</td>
    </tr>
    <tr>
        <td>currentItemId</td>
        <td>当前所在滑块的 item-id ，不能与 current 被同时指定</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td>indicatorDots</td>
        <td>是否显示面板指示点</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>indicatorColor</td>
        <td>指示点颜色</td>
        <td>String</td>
        <td>-</td>
        <td>rgba(0, 0, 0, .3)</td>
    </tr>
    <tr>
        <td>indicatorActiveColor</td>
        <td>当前选中的指示点颜色</td>
        <td>String</td>
        <td>-</td>
        <td>#000000</td>
    </tr>
    <tr>
        <td>loop</td>
        <td>是否环路，仅h5</td>
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
        <td>change</td>
        <td>current 改变时会触发 change 事件</td>
        <td>event.detail = {current: current, source: source}</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
<swiper style="width: 100%; height: 200px;" v-bind:autoplay="formData.autoplay" v-bind:indicatorDots="formData.indicator">
    <swiper-item v-for="pic in pics" style="height: 200px;">
        <axi-image v-bind:src="pic.src" mode="scaleToFill" style="width:100%;height: 100%;" />
    </swiper-item>
</swiper>
```