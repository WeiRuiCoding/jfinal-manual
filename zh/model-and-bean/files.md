BaseModel 是用于被最终的 Model 继承的基类,所有的 getter、setter 方法都将生成在此文 件内,这样就保障了最终 Model 的清爽与干净,BaseModel 不需要人工维护,在数据库有任何 变化时重新生成一次即可。

MappingKit 用于生成 table 到 Model 的映射关系,并且会生成主键/复合主键的配置,也即 在 JFinal 2.1 中无需在 configPlugin(Plugins me)方法中书写任何样板式的映射代码。

DataDictionary 是指生成的数据字典,会生成数据表所有字段的名称、类型、长度、备注、 是否主键等信息。
