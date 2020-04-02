# springboot-mybatis-starter

基于MyBatis-Plus实现代码自动生成的SpringBoot案例

## 实现步骤

1. 基于MySQL建表
    ```sql
    CREATE TABLE IF NOT EXISTS `user`(
       `id` INT UNSIGNED AUTO_INCREMENT,
       `name` VARCHAR(40) NOT NULL,
       `password` VARCHAR(40) NOT NULL,
       `number` VARCHAR(40),
       PRIMARY KEY ( `id` )
    )ENGINE=InnoDB DEFAULT CHARSET=utf8;
    ```

2. 添加MyBatis-Plus依赖
    ```xml
    <dependency>
        <groupId>com.baomidou</groupId>
        <artifactId>mybatis-plus-boot-starter</artifactId>
        <version>3.3.1</version>
    </dependency>
    ``` 