# scrollview
可滚动视图区域。
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
        <td>direction</td>
        <td>滚动方向</td>
        <td>String</td>
        <td>vertical|horizontal</td>
        <td>vertical</td>
    </tr>
    <tr>
        <td>scrollX</td>
        <td>是否允许横向滚动</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>scrollY</td>
        <td>是否允许纵向滚动</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>upperThreshold</td>
        <td>距顶部多远时，触发 scrolltoupper 事件</td>
        <td>Number</td>
        <td>-</td>
        <td>50</td>
    </tr>
    <tr>
        <td>lowerThreshold</td>
        <td>距底部多远时，触发 scrolltolower 事件</td>
        <td>Number</td>
        <td>-</td>
        <td>50</td>
    </tr>
    <tr>
        <td>enableBackToTop</td>
        <td>点击系统状态栏是否滚动至顶部</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>scrollWithAnimation</td>
        <td>是否在设置滚动条位置时使用动画过渡</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>scrollIntoView</td>
        <td>值应为某子元素id（id不能以数字开头）。设置哪个方向可滚动，则在哪个方向滚动到该元素</td>
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
        <td>scrolltoupper</td>
        <td>滚动到顶部触发</td>
        <td>-</td>
    </tr>
    <tr>
        <td>scrolltolower</td>
        <td>滚动到低部触发</td>
        <td>-</td>
    </tr>
    <tr>
        <td>scroll</td>
        <td>滚动时触发</td>
        <td>event.detail = {scrollLeft, scrollTop, scrollHeight, scrollWidth, deltaX, deltaY}</td>
    </tr>
</table>
<h2 id="cid_2">示例</h2>

```html
 <axi-textarea maxlength="-1" class="rich-text-editor"  v-model:text="htmlSnip"></axi-textarea>
 <!-- 小程序rich-text在组件内部则样式不生效，只有在page内才生效，如果html中使用了样式建议直接使用rich-text -->
 <rich-text v-if="env==='miniprogram'" v-bind:nodes="htmlSnip"></rich-text>
```