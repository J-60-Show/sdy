# Hibernate注解之@Enumerated
@Enumerated(value=EnumType.ORDINAL)采用枚举类型的序号值与数据库进行交互，
此时数据库的数据类型需要是数值类型，例如在实际操作中

```
CatTest ct = new CatTest();
ct.setColor(Color.BLUE);
```

当我们将对象gt保存到数据库中的时候，数据库中存储的数值是BLUE在Color枚举
定义中的序号1(序号从零开始)；


@Enumerated(value=EnumType.STRING)采用枚举类型与数据库进行交互，
此时数据库的数据类型需要是NVACHAR2等字符串类型，例如在实际操作中

```
CatTest ct = new CatTest();
ct.setColor(Color.BLUE);
```
数据库中存储的数值是BLUE字符串。
