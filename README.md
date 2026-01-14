# SQL-Notes

个人 SQL / DuckDB 学习仓库（投资组合分析为主）

## 目录
- `recipes/` 任务型“菜谱”SQL（可直接复制粘贴跑）
- `concepts/` 概念与常见坑（JOIN、窗口函数、日期处理…）
- `notebooks/` 可运行的 Jupyter/Markdown
- `data/` 小样例数据
- `cheatsheets/` 速查清单

## 快速开始
- Jupyter: `%load_ext sql` → `%sql duckdb:///:memory:`
- DuckDB 读 CSV:  
  ```sql
  CREATE TABLE prices AS
  SELECT * FROM read_csv_auto('data/prices_sample.csv');
