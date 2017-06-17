# 对象 Service
系统服务管理对象

## 构造函数
        
### Service
系统服务管理对象构造函数
```JavaScript
 new Service(String name,
                Function worker,
                Object event = {});
```

** 调用参数: **
* name - 服务名称
* worker - 服务运行函数
* event - 服务事件处理

## 函数
        
### install
安装服务到系统
```JavaScript
Service.install(String cmd,
                String displayName = "",
                String description = "");
```

** 调用参数: **
* cmd - 服务命令行
* displayName - 服务显示名称
* description - 服务描述信息

### remove
从系统中卸载服务
```JavaScript
Service.remove();
```

### start
启动服务
```JavaScript
Service.start();
```

### stop
停止服务
```JavaScript
Service.stop();
```

### restart
重启服务
```JavaScript
Service.restart();
```

### run
开始运行服务实体
```JavaScript
Service.run();
```

### isInstalled
检测服务是否安装
```JavaScript
Boolean Service.isInstalled();
```

** 返回结果:**
* 服务安装返回 True

### isRunning
检测服务是否运行
```JavaScript
Boolean Service.isRunning();
```

** 返回结果:**
* 服务运行返回 True

### on
绑定一个事件处理函数到对象
```JavaScript
Object Service.on(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回成功绑定的数量，如果函数已绑定则返回 0

### on
绑定一个事件处理函数到对象
```JavaScript
Object Service.on(Object map);
```

** 调用参数: **
* map - 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### addListener
绑定一个事件处理函数到对象
```JavaScript
Object Service.addListener(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### addListener
绑定一个事件处理函数到对象
```JavaScript
Object Service.addListener(Object map);
```

** 调用参数: **
* map - 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### prependListener
绑定一个事件处理函数到对象起始
```JavaScript
Object Service.prependListener(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回成功绑定的数量，如果函数已绑定则返回 0

### prependListener
绑定一个事件处理函数到对象起始
```JavaScript
Object Service.prependListener(Object map);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回成功绑定的数量，如果函数已绑定则返回 0

### once
绑定一个一次性事件处理函数到对象，一次性处理函数只会触发一次
```JavaScript
Object Service.once(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### once
绑定一个一次性事件处理函数到对象，一次性处理函数只会触发一次
```JavaScript
Object Service.once(Object map);
```

** 调用参数: **
* map - 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### prependOnceListener
绑定一个事件处理函数到对象起始
```JavaScript
Object Service.prependOnceListener(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回成功绑定的数量，如果函数已绑定则返回 0

### prependOnceListener
绑定一个事件处理函数到对象起始
```JavaScript
Object Service.prependOnceListener(Object map);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回成功绑定的数量，如果函数已绑定则返回 0

### off
从对象处理队列中取消指定函数
```JavaScript
Object Service.off(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### off
取消对象处理队列中的全部函数
```JavaScript
Object Service.off(String ev);
```

** 调用参数: **
* ev - 指定事件的名称

** 返回结果:**
* 返回事件对象本身，便于链式调用

### off
从对象处理队列中取消指定函数
```JavaScript
Object Service.off(Object map);
```

** 调用参数: **
* map - 指定事件映射关系，对象属性名称作为事件名称，属性的值作为事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### removeListener
从对象处理队列中取消指定函数
```JavaScript
Object Service.removeListener(String ev,
                Function func);
```

** 调用参数: **
* ev - 指定事件的名称
* func - 指定事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### removeListener
取消对象处理队列中的全部函数
```JavaScript
Object Service.removeListener(String ev);
```

** 调用参数: **
* ev - 指定事件的名称

** 返回结果:**
* 返回事件对象本身，便于链式调用

### removeListener
从对象处理队列中取消指定函数
```JavaScript
Object Service.removeListener(Object map);
```

** 调用参数: **
* map - 指定事件映射关系，对象属性名称作为事件名称，属性的值作为事件处理函数

** 返回结果:**
* 返回事件对象本身，便于链式调用

### removeAllListeners
从对象处理队列中取消所有事件的所有监听器， 如果指定事件，则移除指定事件的所有监听器。
```JavaScript
Object Service.removeAllListeners(Array evs = []);
```

** 调用参数: **
* evs - 指定事件的名称

** 返回结果:**
* 返回事件对象本身，便于链式调用

### setMaxListeners
监听器的默认限制的数量，仅用于兼容
```JavaScript
Service.setMaxListeners(Integer n);
```

** 调用参数: **
* n - 指定事件的数量

### getMaxListeners
获取监听器的默认限制的数量，仅用于兼容
```JavaScript
Integer Service.getMaxListeners();
```

### listeners
查询对象指定事件的监听器数组
```JavaScript
Array Service.listeners(String ev);
```

** 调用参数: **
* ev - 指定事件的名称

** 返回结果:**
* 返回指定事件的监听器数组

### listenerCount
查询对象指定事件的监听器数量
```JavaScript
Integer Service.listenerCount(String ev);
```

** 调用参数: **
* ev - 指定事件的名称

** 返回结果:**
* 返回指定事件的监听器数量

### eventNames
查询监听器事件名称
```JavaScript
Array Service.eventNames();
```

** 返回结果:**
* 返回事件名称数组

### emit
主动触发一个事件
```JavaScript
Boolean Service.emit(String ev,
                ...);
```

** 调用参数: **
* ev - 事件名称
* ... - 事件参数，将会传递给事件处理函数

** 返回结果:**
* 返回事件触发状态，有响应事件返回 true，否则返回 false

### dispose
强制回收对象，调用此方法后，对象资源将立即释放
```JavaScript
Service.dispose();
```

### equals
比较当前对象与给定的对象是否相等
```JavaScript
Boolean Service.equals(object expected);
```

** 调用参数: **
* expected - 制定比较的目标对象

** 返回结果:**
* 返回对象比较的结果

### toString
返回对象的字符串表示，一般返回 &#34;[Native Object]&#34;，对象可以根据自己的特性重新实现
```JavaScript
String Service.toString();
```

** 返回结果:**
* 返回对象的字符串表示

### toJSON
返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合
```JavaScript
Value Service.toJSON(String key = "");
```

** 调用参数: **
* key - 未使用

** 返回结果:**
* 返回包含可 JSON 序列化的值

### valueOf
返回对象本身的数值
```JavaScript
Value Service.valueOf();
```

** 返回结果:**
* 返回对象本身的数值

## 属性
        
### name
查询和设置服务名称
```JavaScript
String Service.name;
```

### onstop
查询和绑定服务停止事件，相当于 on(&#34;stop&#34;, func);
```JavaScript
Function Service.onstop;
```

### onpause
查询和绑定服务暂停事件，相当于 on(&#34;pause&#34;, func);
```JavaScript
Function Service.onpause;
```

### oncontinue
查询和绑定服务恢复事件，相当于 on(&#34;continue&#34;, func);
```JavaScript
Function Service.oncontinue;
```

### defaultMaxListeners
默认全局最大监听器数
```JavaScript
Integer Service.defaultMaxListeners;
```
