1. **简单查询**：列出所有笔记的标题。

```dataview
TABLE title
FROM "Dataview-Example"
```

2. **按标签查询**：查找所有带有“学习”标签的笔记。

```dataview
TABLE title, date
FROM ""
WHERE contains(tags, "学习")
```

3. **按日期排序**：按日期排序列出笔记。

```dataview
TABLE title, date
FROM ""
SORT date DESC
````

4. **任务查询**：查找所有未完成的任务。

```dataview
TASK
from "Dataview-Example"
WHERE !completed
```

### 使用技巧

- **调试查询**：如果查询没有返回结果，检查你的 YAML 格式和字段名称。
- **自定义视图**：尝试不同的视图类型，如 LIST 或 CALENDAR，以更好地展示数据。
