
# 模组内容

## Action：ModifyCVarExpanded

与原版ModifyCVar用法一致，但增加了传递自身变量的功能，使用@ + 变量名即可将自身的变量推送给target，当然也可以只推送常量。

```xml
<!-- 使用示例 推送变量 -->
<triggered_effect trigger="[TRIGGER]" action="ModifyCVarExpanded" target="[OTHER]" cvar="[CVAR]" operation="[OPERATION]" value="@[VALUE]" />

<!-- 或推送常量 -->
<triggered_effect trigger="[TRIGGER]" action="ModifyCVarExpanded" target="[OTHER]" cvar="[CVAR]" operation="[OPERATION]" value="[VALUE]" />
```

## Action：RefreshBuffDisplay

要求提供参数buff，值即为buff的name，作用是刷新buff的名字等状态，相当于将buff删除再重新加会时对ui进行的更新操作（并不会真的将buff删除再加回）

```xml
<!-- 使用示例 -->
<triggered_effect trigger="[TRIGGER]" action="RefreshBuffDisplay" buff="[BUFF]"/>
```
