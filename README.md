# AK-Design 可视化低代码快速开发平台

AK-Design 是一个纯前端的`拖拽式`、`可视化`、`低代码`数据可视化设计器开发平台，主包括表单设计、列表页设计、流程设计、数据可视化大屏设计、数据统计设计

使用基于 Vue 3.x 的桌面端组件库 Elemnet-Plus ，使用广泛，扩展方便

通过可视化的操作，可轻松快速完成表单设计、列表页设计、流程管理设计、数据可视化屏设计、数据统计设计等页面的创建

提供功能强大的各类组件，可适用在各种复杂的场景中

代码简洁、易于二次开发

用于学习研究，欢迎交流，微信：**337547038**

如果项目对你有所帮助，请点赞+关注，以防迷路

如果你对该项目感兴趣，欢迎加入项目建设中来

如果你有任何建议，请联系我或在评论区留言

## 表单设计

一种可视化拖拽式表单设计编辑器，能够以图形化方式生成表单。通过它，可以以无需编写代码的方式来构建表单，并且可以为表单添加各种校验规则。
设计器具有易用性，且能够为应用程序快速生成美观的表单，提高开发效率。

设计器的主要功能：

- 提供功能强大丰富的各种表单组件

- 可以使用拖放方式添加表单元素

- 可以使用鼠标进行表单元素排序

- 可以设计器预设的校验规则

- 可以生成完整的表单视图

- 可以生成表单数据

- 可以根据表单数据自动生成UI

- 可以根据表单模板快速生成表单

- 可以支持复杂交互控制

- 可以支持开发自定义组件

- 支持接口数据处理

...

## 列表设计

列表设计器是一个可以帮助快速构建数据展示界面的工具，可以更加轻松地实现列表构建，提高我们的工作效率。简单的拖拽、调整列顺序、编辑列、设置样式等，生成自己想要的数据表格。
还可从设计的表单里获取接口数据。

列表设计器提供了丰富的配置项，你可以进行列的拖拽、设置列名、设置列宽、设置列样式等操作。同时，它还提供了丰富的配置项，充足的自定义能力，能够满足我们大部分的需求。

## 流程设计

## 数据可视化大屏设计

提供一种简单易用的拖拽式数据可视化大屏设计方案。编辑器提供了丰富的组件库和多种样式配置选项，可以帮助用户快速搭建并定制属于自己的数据可视化大屏。

包括图表组件、表格组件、进度条组件、地图组件、轮播组件、背景边框组件和常用辅助工具等，用户可以根据自己的需求选择和拖拽组件到画布中。

- 编辑器页面基本功能，包括编辑、预览、导出、保存、生成json脚本
- 图层功能：显示、隐藏、复制、锁定
- 组件功能：缩放、旋转、拖动、复制、组合、拆分、对齐方式、删除、位置定位
- 支持用户自定义组件
- 支持接口数据和静态模拟数据
- 支持键盘调整定位

## 数据统计设计

### 目录结构

```text
public
 ├─mock // 模拟数据
src
 ├─api // 数据请求接口
 ├─docs // 使用说明文档
 └─views // 页面
   ├─design // 表单设计主程序组件
     ├─components // 公共组件
     ├─dataList // 列表页设计
     ├─dataScreen // 数据大屏设计
     ├─dataSource // 数据源设计
     ├─flow // 流程设计
     └─form // 表单设计
   └─system // 系统框架基本页面，导出vue文件示例
```

### 启动项目

```Bash

# 克隆项目
git clone https://github.com/337547038/vue-form-design.git

# 安装依赖
pnpm install

# 运行项目
pnpm dev

# 使用json模拟数据（建议使用node模拟接口，方法见启动node模拟接口）

 将/src/api/index.ts约25行 
 if (window.location.host.indexOf('github') !== -1)中的github
 修改为你本地运行的地址如 localost或192.128.xx
 
# 打包项目
pnpm build

```

### 启动node模拟接口

```Bash

1.将/src/nodejs/akform.sql导入mysql中

2./src/nodejs/db.js修改连接数据库用户密码相关信息

# 进入nodejs目录

cd nodejs

# 安装依赖

pnpm install

#运行项目

pnpm dev

```

### 开发环境
| 名称           | 版本      |
|--------------|---------|
| node         | 16.15.x |
| pnpm         | 8.6.x   |
| vite         | 4.3.x   |
| vue          | 3.2.x   |
| element-plus | 2.3.x   |

### 贡献者
