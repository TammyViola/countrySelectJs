# countrySelectJs

#### 介绍
国家/地区选择插件，可以显示英文或中文，包含输入过滤等。
当前版本1.0，国家/地区数据源更新时间：2025.04.07

#### HTML 调用
	<html>
		<head>
			<link href="./dist/css/countrySelect.css" rel="stylesheet" type="text/css"/>
		</head>

		<body>
			<!-- 被绑定的控件 -->
			<input type="text" id="countryInput" placeholder="选择国家/地区">
		</body>

		<script type="text/javascript" src="./dist/js/countrySelect.min.js"></script>
	</html>

#### JS调用方法

	<script type="text/javascript">
		// 使用示例
		const countrySelector = new CountrySelector({
	    inputId: 'countryInput',  // 绑定的input的id
	    language: 'zh', // 或 'en'
	    showFlag: true,  // 是否显示国旗图标
	    preferredCountries: ['CN', 'US'], // 优先显示的国家
	    excludedCountries: ['TW'], // 排除中国台湾
	    defaultValue: 'CN', // 设置默认值为中国
	    enableSearch: true, // 启用搜索功能
	    showDivider: true // 显示分隔线
  	});
	</script>

#### 具体说明
https://www.cnblogs.com/TammyBlog/p/18814258