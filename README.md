# 2018web-apply
<h2>vue双向绑定-object.defineProperty()</h2>
<p>
	vue.js 则是采用数据劫持结合发布者-订阅者模式的方式，通过Object.defineProperty()来劫持各个属性的setter，getter，在数据变动时发布消息给订阅者（文本节点则是作为订阅者），在收到消息后执行相应的更新操作。
	对象：无序属性的集合，键值对集合。
	对象属性分为数据属性访问器属性，数据属性就是普通的属性，例如一个实例对象person的name，age等
<pre>
var person = {
	name: 'tfciw',
	age: 25
}
name等就是数据属性，es5规定了描述其行为的特性，configurable,enumerable,writable,value,是否可以通过delete删除重新定义该属性，是否可以被for-in枚举，能否修改该属性的值，值。
默认：true，true，true，undefined。
要想修改属性的特性必须使用object.defineProperty();该方法接受三个参数，属性所属的对象名称，属性名称，描述对象。描述对象只能是上面四个特性一部分或全部。
object.defineProperty(person,name,{
	configurable: true,
	value: 'tfciwjyl'
})
</pre></p>
<h2>animation</h2>
<p>
	transform: 旋转rotate、缩放(scale)、移动(translate)或倾斜skew
	transform: translate(10px) -> 元素x轴向右平移10px
	transform: translate(10px, 10px) -> 元素x轴向右y轴向下平移10px，可支持负值
</p>
