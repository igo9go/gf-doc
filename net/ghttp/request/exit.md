
# `Exit`, `ExitAll`与`ExitHook`

1. `Exit`: 仅退出当前执行的逻辑方法，如: 当前`HOOK`方法、服务方法，不退出后续的逻辑处理，可用于替代`return`；
1. `ExitAll`: 强行退出当前执行流程，当前执行方法的后续逻辑以及后续所有的逻辑方法将不再执行，常用于权限控制；
1. `ExitHook`: 当路由匹配到多个`HOOK`方法时，默认是按照路由匹配优先级顺序执行`HOOK`方法。当在`HOOK`方法中调用`ExitHook`方法后，后续的`HOOK`方法将不会被继续执行，作用类似`HOOK`方法覆盖；
1. 这三个退出函数仅在服务函数和`HOOK`事件回调函数中有效，无法控制中间件的执行流程；