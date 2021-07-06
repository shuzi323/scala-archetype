# 制作archetype
参考https://www.freesion.com/article/24491052853/
1. 首先在项目根目录执行`mvn archetype:create-from-project`
2. 之后会在`target/generated-sources/archetype`下面生成一个pom.xml文件
3. 在`target/generated-sources/archetype` 目录下执行`mvn install`
4. 在`.m2/repository`目录下增加了archetype的 pom.xml 文件（可以更改其artifactId和 name 改成自己想要的）
5. 然后在一个新的空文件夹下面用刚才安装的archetype构建项目即可