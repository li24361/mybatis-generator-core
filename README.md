修改部分
> * 修复乱码问题，生成文件一律转为utf-8

> * 修改配置catalog时，生成代码为Schema..table的问题 
因为mysql不建议跨数据库调用，所以，Generator生成的时候，不支持生成S61.T6110这种，只会生成S61..T6110，所以每次还要替换一下
原因参考https://github.com/mybatis/generator/issues/17


> * 修改生成注释类，将英文注释去掉，改为数据库字段注释
