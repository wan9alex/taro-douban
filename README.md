# taro-douban
测试收集用法
------------------------------------------------------------
taro规范:
	UI组件： 类小程序标签（大驼峰）
	page/components: 类组件
	this修正 时 不用匿名函数 ?
	内置组件（小程序组件）引入后再使用
	支持使用 CSS 预编译处理器，目前提供了 sass 预编译插件 @tarojs/plugin-sass，需要自行在本地进行安装
	this.$router.params 抓取页面参数,跳转通过API，组件没实现
	用react钩子，小程序钩子能用，但H5下失效
	嵌套的是component组件，跳转的是pages，组件有componentWillReceiveProps钩子，页面没有
	jsx中不适应延展操作...
	页面和组件类中，this 指向的是 Taro 页面或组件的实例
	组件传递函数属性名以 on 开头  <Custom onTrigger={this.handleEvent}></Custom>
	Taro.api() 打包了所有小程序API，异步api 可promise方式使用
	状态管理：redux + @tarojs/redux == react-redux
		https://nervjs.github.io/taro/docs/redux.html

	app.json/page.json -> app.js/page.js(config)
