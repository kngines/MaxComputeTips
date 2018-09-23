#### 1. 切换项目
- ``` use project_name; ```

#### 2. 查询所有表
- ``` list tables; ```

#### 3. 查看表所有分区
- ``` ls partitions tablename; ```

#### 4. 查看表所有分区
- ``` ls partitions tablename; ```

#### 5. 查看表结构
- ``` desc tablename; ```

#### 6. 获取json列函数
- ``` get_json_object(src,value) ```
    - eg. ```get_json_object(columnName,'$.importance.com_city.rank')```
    
#### 7. 模糊查询部分表
- ``` show tables like 'test*'; ```

#### 8. 将文件数据加载到表
- ``` tunnel upload -fd '\t' c:\file.txt table_name; ```

#### 9. 将表数据导出至文件
- ``` tunnel d table_name c:\file.txt; ```