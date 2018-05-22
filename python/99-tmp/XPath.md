# XPath

选取节点

XPath 使用路径表达式在 XML 文档中选取节点。节点是通过沿着路径或者 step 来选取的。

下面列出了最有用的路径表达式：

表达式 | 描述
----|---
nodename | 选取此节点的所有子节点。
/ | 从根节点选取。
// | 从匹配选择的当前节点选择文档中的节点，而不考虑它们的位置。
. | 选取当前节点。
.. | 选取当前节点的父节点。
@ | 选取属性。