### MaxCompute(ODPS) SQL Tips

#### 1. 日期行为汇总
- 汇总每天、近3日、近7日pv量
    - ``` 
        SELECT id
           , SUM(IF(ds = '${ds}', pv, 0)) AS today_pv -- 当日pv
           , SUM(IF(ds > '${ds3}', pv, 0)) AS 3_days_pv  -- 近3日pv
           , SUM(pv) AS 7_days_pv    -- 近7日pv
        FROM pv_daily_table
        WHERE ds > '${ds7}' and ds <= '${ds}'
        GROUP BY id;
      ```
      
#### 2. 日期行为汇总
- 汇总每天、近3日、近7日pv量
    - ``` 
        SELECT id
           , SUM(IF(ds = '${ds}', pv, 0)) AS today_pv -- 当日pv
           , SUM(IF(ds > '${ds3}', pv, 0)) AS 3_days_pv  -- 近3日pv
           , SUM(pv) AS 7_days_pv    -- 近7日pv
        FROM pv_daily_table
        WHERE ds > '${ds7}' and ds <= '${ds}'
        GROUP BY id;
      ```