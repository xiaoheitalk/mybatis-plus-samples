
参考https://baomidou.com/pages/42ea4a/
1. 继承com.baomidou.mybatisplus.core.injector.AbstractMethod，实现injectMappedStatement方法
2. 继承com.baomidou.mybatisplus.core.injector.DefaultSqlInjector，将上一步的方法实例增加到MethodList中
3. 继承com.baomidou.mybatisplus.core.mapper.BaseMapper，定义上面的方法