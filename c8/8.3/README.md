# 8.3 使用构建工具自动化例行工作
&emsp;&emsp;因为JavaScript是解释型语言，所以不需要编译，只需要配置好源代码就可以直接运行了，这样的便捷性也是其优点。但是，近年来，JavaScript的开发越来越复杂了。例如，运行JavaScript的代码，通常伴随着以下的工作。
- 如果使用了altJS（P.278），需要编译
- 执行单元测试（8.1节）
- 使用JSLint（http://www.jslint.com/ ）进行代码检查
- 压缩源代码

&emsp;&emsp;虽然这些工作都不是很难。但是，如果让人在开发过程中执行多次，多少会有遗漏或者错误。因此，构建工具Grunt（也称为Task Runner）的功能便是让这些工作实现自动化。如果有其他语法开发经验的人，想象一下「Ant／Maven（Java）、make这样的」便容易理解了。在JavaScript中，Gulp（http://gulpjs.com ）也是类似的工具。