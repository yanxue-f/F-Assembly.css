>*欢迎查看前端新人“焱雪”的组件库*
# F-assembly
纯粹的css组件库


##  1.24栅栏布局组件

* row 类：用于创建flex布局环境。
* col 类：用于布局时，编辑row元素下的子元素的文件长度。
* no-stackable 类：设置于row类元素上，实现文件的自适应长度展示，不加此类名可实现堆积展示。
* justify 类：设置于row类元素上，用于实现col类元素主轴方向的对齐方式，有头部对齐，尾部对齐，居中对齐，不同间距的两边对齐。
* align 类：设置于row类元素上，用于实现col类元素交叉轴方向的对齐方式，有顶部对齐，底部部对齐，居中对齐。
* align-self 类：设置于col类元素上，用于实现col类元素自己交叉轴方向的对齐方式，有顶部对齐，底部部对齐，居中对齐。
* offset 类：设置col类元素上，用于设置col类元素距离左侧的间隔，会影响后续col类元素。
* push 类：设置col类元素上，用于设置col类元素向右移动的距离，不影响其他元素。
* pull 类：设置col类元素上，用于设置col类元素向左移动的距离，不影响其他元素。
* gutter 类：设置于row类元素上，用于设置col类元素列和横的间距。可用gutter同时设置，也可用gutter-column和gutter-row分别设置列间距和行间距。
* order 类： 用于设置col类元素的分布顺序，order数值越小越靠前，一般都要设置。默认为0.
* 响应式布局：不同布局下遵顼不同的布局方式，justify、col、offset、align、align-self、gutter、push、pull、order均可响应，许分别加上xs、sm、md、lg、xl、xxl的后缀加需要设置的number。
* 分别对应：
    - xs 屏幕 < 576px
    - sm 屏幕 ≥ 576px
    - md 屏幕 ≥ 768px
    - lg 屏幕 ≥ 992px
    - xl 屏幕 ≥ 1200px
    - xxl 屏幕 ≥ 1600px

演示: [24 layout] <https://fan-aoqiang.gitee.io/f-assembly.css/24layout/>

## 2.Split line

* divider类：创建分割线的生成环境。
* divider-row类：配合divider类实现水平分割线，可加文字。
* divider-column类：配合divider类实现垂直分割线，可加入文字。
* text-position-()类：设置分割线上的文本位置，默认在文本开头位置，text-position-center：在文本居中位置，text-position-end：在文本末尾位置。
* linear-()类：改变分割线的线性，默认为实线，linear-dotted：点状线。linear-dashed：虚线。
* divider-inline类：配合divider类实现行内分割线。
* divider-night类：配合divider类实现夜间模式下的分割线。
* 改变分割线的样式：通过改变divider类divider-row类和divider-colum类显得gap，font-size，font，border-bottom，border-right属性来改变分割线的样式。
演示: [Splitline] <https://fan-aoqiang.gitee.io/f-assembly.css/Splitline/>.

## 3.radio

* radio类：基本单选框用id于for将input和label组合。
* radio禁用状态：radio在disabled和checked，disabled下的状态。
* radio组合：用相同的name组合。
* radio-block类:单选框垂直排布。
* radio的大小：使用radio-content配合radio-large，radio-small实现不同大小的文字单选框。
* radio的样式：使用radio-circular，radio-content和radio-fill实现不同的单选框。
* 自定义单选框:通过改变radio或radio-block下的变量：--radio ，--radio-color ，--radio-shadow的值来改变单选框的样式。通过改变radio或radio-block下的gap属性改变文字距离圆点的距离。

演示: [radio] <https://fan-aoqiang.gitee.io/f-assembly.css/radio/>.

## 4.checkbox

* checkbox类：基本多选框用id于for将input和label组合。
* checkbox禁用状态：checkbox在disabled和checked，disabled下的状态。
* checkbox组合：用相同的name组合。
* checkbox-block类:多选框垂直排布。
* checkbox的大小：使用rcheckbox-content配合checkbox-large，checkbox-small实现不同大小的文字多选框。
* checkbox的样式：使用checkbox-frame，checkbox-content和checkbox-fill实现不同的多选框。
* 自定义多选框:通过改变checkbox或checkbox-block下的变量：--checkbox ，--checkbox-color ，--checkbox-shadow的值来改变多选框的样式。通过改变checkbox或checkbox-block下的--checkbox改变文字距离方片的距离。

演示:  [checkbox] <https://fan-aoqiang.gitee.io/f-assembly.css/checkbox/>

## 5.button

* 基础按钮：在button标签中添加button类来实现基础按钮，而后通过添加各种不同的类名来实现不同的按钮样式。
* plain类代表朴素类型的按钮，round类代表圆角类型按钮，circle代表圆形图标按钮（不包含文字需要插入相应的图片）。
*  button-default类代表默认按钮(透明)
* button-main类代表圆角主要按钮（蓝色）
* button-success代表圆形成功按钮（绿色）
* button-info代表圆形信息按钮（灰色）
* button-warn类代表警告按钮(橙色)
* button-danger类代表危险按钮(红色)。
* 禁用状态：通过为button类元素添加disabled属性实现禁用按钮。
* 文本按钮：没有边框和背景色的按钮,通过为button类元素添加button-text类实现纯文本按钮。
* 图标按钮:使用图标为按钮添加更多的含义,你也可以单独使用图标不添加文字来节省显示区域占用。
* 加载状态按钮：点击按钮处于加载状态，向用户反馈数据的情况。
* 各种尺寸的尺寸按钮：除了默认的大小，按钮组件还提供了几种额外的尺寸可供选择，以便适配不同的场景。

演示: [checkbox] <https://fan-aoqiang.gitee.io/f-assembly.css/Button/>
