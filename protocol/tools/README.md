# Tools

A guide for tools we are using within 孜点.

## [钉钉](https://im.dingtalk.com/)
For discussion.

## [Trello](https://trello.com/)
(Product)Project management.

## [GitHub](https://github.com/)
(Development)Project management and collaborate.

## [腾讯文档](docs.qq.com/)
Sharing and collaborating docs and sheets.

在腾讯文档提供团队管理以及文件夹功能之前，使用统一的命名格式来保持文档目录的规范。要求如下：

> 孜点-[部门名称]?-[项目名称]-[内容描述]..-[相关人员姓名]?..-[版本标识]?-[日期]?

格式说明：

1. 完整文件名由多部分组成，以`-`间隔（无空格）
2. 特殊字符说明：
    - 方括号`[]`中表示动态可替换内容，实际文件名并不包含`[]`
    - 无`[]`则表示固定内容，如`孜点`为所有文档前缀。
    - `[]?`表示该部分内容可选
    - `[]..`表示该部分可能包含多个同类内容，可用于细化描述内容或将大项目拆分为多个文档，如：`孜点-寻鹿高考-开发文档]-UI`, `孜点-寻鹿高考-开发文档-后端`, `孜点-寻鹿高考-开发文档-数据`
    - 特殊符号后缀（`?` `..`)可组合，如`[相关人员]?..` 表示可能此部分既可以省略也可能包含1到多位相关人员
3. 日期格式为8位数字不包含任何非数字字符，如：20180518
4. 只使用英文标点符号且避免多余空格（如首尾）
5. 对同一事物保持在多个文档下用词统一，如部门名称、项目名称，以及字母大小写始终一致

一些文件命名示例：

- `孜点-寻鹿高考-设计优化反馈-v1.2.5-20180518`
- `孜点-技术开发部-寻鹿高考-开发文档`

## [DiffMerge](https://www.sourcegear.com/diffmerge/)
Visually compare and merge files