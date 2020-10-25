---
description: Mysql库表结构
---

# 数据库设计库表结构

## 数据库文档

**数据库名：** bookmanagement

**文档版本：** 1.0-SNAPSHOT

**文档描述：** 数据库文档生成

| 表名 | 说明 |
| :--- | :--- |
| book | 书本信息表 |
| borrow |  |
| user |  |

**表名：** book

**说明：** 书本信息表

**数据列：**

| 序号 | 名称 | 数据类型 | 长度 | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | id | int | 10 | 0 | N | Y |  |  |
| 2 | bookid | varchar | 255 | 0 | N | N |  |  |
| 3 | name | varchar | 255 | 0 | N | N |  |  |
| 4 | press | varchar | 255 | 0 | Y | N |  |  |
| 5 | publishdate | datetime | 19 | 0 | Y | N |  |  |
| 6 | author | varchar | 255 | 0 | N | N |  |  |
| 7 | content | varchar | 255 | 0 | Y | N |  |  |
| 8 | stock | int | 10 | 0 | Y | N | 0 |  |
| 9 | total | int | 10 | 0 | Y | N |  |  |

**表名：** borrow

**说明：**

**数据列：**

| 序号 | 名称 | 数据类型 | 长度 | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | id | int | 10 | 0 | N | Y |  |  |
| 2 | uid | int | 10 | 0 | N | N |  |  |
| 3 | bid | int | 10 | 0 | N | N |  |  |
| 4 | btime | datetime | 19 | 0 | N | N |  |  |
| 5 | bdays | int | 10 | 0 | Y | N | 0 |  |
| 6 | returntime | datetime | 19 | 0 | Y | N |  |  |

**表名：** user

**说明：**

**数据列：**

| 序号 | 名称 | 数据类型 | 长度 | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | id | int | 10 | 0 | N | Y |  |  |
| 2 | name | varchar | 255 | 0 | Y | N |  |  |
| 3 | password | varchar | 255 | 0 | Y | N |  |  |
| 4 | stud | varchar | 255 | 0 | Y | N |  |  |
| 5 | dept | varchar | 255 | 0 | Y | N |  |  |
| 6 | grade | varchar | 40 | 0 | Y | N |  |  |
| 7 | gender | varchar | 4 | 0 | N | N |  |  |

