# labreport-cs

## 目的

实验报告 LaTeX 模版。

## 内容

`labreport.cls`。

## 使用方法

直接将其放入文档的根目录，随后在待编译的`.tex`的导言区内导入文档类
```
\documentclass{labreport}
```

## 设置方法

本模版使用 Key-Value 方式来填写信息、设置字体。具体设置内容如下所示。

```
\labreportSetup
  {
    info = {
      ...
    }, 
    style = {
      ...
    }
  }
```

### `info`设置

- `courseName  = {<课程名称>},`，在花括号内填入课程名称；
- `teacherName = {<指导教师>},`，在花括号内填入指导教师；
- `labName     = {<上机实践名称>},`，在花括号内填入上机实践名称；
- `labNo       = {<上机实践编号>},`，在花括号内填入上机实践编号；
- `studentID   = {<学号>},`，在花括号内填入学号；
- `name        = {<姓名>},`，在花括号内填入姓名；
- `grade       = {<年级>},`，在花括号内填入年级；
- `groupNo     = {<组号>},`，在花括号内填入组号；
- `date        = {<日期>},`，在花括号内填入日期；
- `time        = {<课时数>},`，在花括号内填入课时数。

### `font`设置

- `fontEN        = lm | times | default, `，英语字体选项，选项意思依次为 Latin Modern，Times，以及默认（选择默认时为`times`）；
- `fontMath      = lm | times | default,`，数学字体选项，选项意思依次为 Latin Modern，Times，以及默认（选择默认时为`lm`）。
