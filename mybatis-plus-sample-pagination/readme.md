# page

### 分页插件

```
@Bean
    public MybatisPlusInterceptor mybatisPlusInterceptor() {
        MybatisPlusInterceptor interceptor = new MybatisPlusInterceptor();
        interceptor.addInnerInterceptor(new PaginationInnerInterceptor(DbType.H2));
        return interceptor;
    }
```

## 特性

* 按照查询属性进行排序：OrderItem#asc， OrderItem#desc



## 示例

### testMyPageMap

返回的结果为page时，会对sql先进行count(*)操作



### myPage

参数为page及其子类时，会先对sql先进行count(*)操作