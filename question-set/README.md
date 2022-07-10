# 题组  
`NextTest` 中可以有多个`题库`，每个`题库`可以提供自己的`题组`结构。

`NextTest` 的所有数据使用 [`YAML`](https://yaml.org/) 结构。

# 版本
目前最新的版本为 `v1`。
```
https://nexttest-schemas.xfqlittlefan.xyz/question-set/v1.json
```

# 参考
## 1. `version` 模板版本
一个整数。为模板版本去掉 `v`。如 `1`。

## 2. `information` 题组信息
一个对象。

### 2.1. `title` 标题
一个字符串。

### 2.2. `description` 描述
一个字符串。

### 2.3. `version` 版本
一个字符串。示例：`1.0.0+1`。\+ 号前使用[语义化版本](https://semver.org/lang/zh-CN/)，+ 号后为版本号。`NextTest` 使用版本号判断版本大小。

### 2.4. `author` 题组作者
一个字符串。

## 3. `questions` 题目列表

一个数组，接受对象。