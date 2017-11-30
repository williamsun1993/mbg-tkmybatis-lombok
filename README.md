# mbg-tkmybatis-lombok
MyBatis Generator使用说明
该工具用于连接数据库生成POJO和Mapper接口，生成的POJO基于lombok，生成的Mapper接口基于tk.MyBatis。
操作步骤：

##1. 配置数据库连接信息
generatorConfig.xml -> 找到generatorConfiguration下的jdbcConnection，修改connectionURL，userId，password部分为要连接的数据库信息。

##2. 修改POJO类生成的位置
generatorConfig.xml -> 找到generatorConfiguration下的javaModelGenerator，修改targetPackage（生成的包名）。

##3. 修改Mapper接口生成的位置、
generatorConfig.xml -> 找到generatorConfiguration下的javaClientGenerator，修改targetPackage（生成的包名）。

##4. 运行，获取生成的文件
Run-> GeneratorSqlmap.mian()方法，然后在1, 2步骤配置的路径中即可获取生成的相关文件。

# Link
- tk.MyBatis https://github.com/abel533/Mapper
- Mybatis Generator https://github.com/mybatis/generator
- lombok https://github.com/rzwitserloot/lombok
