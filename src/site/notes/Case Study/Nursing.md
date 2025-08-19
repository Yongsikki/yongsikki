---
{"dg-publish":true,"permalink":"/case-study/nursing/","created":"2025-07-22T18:31:14.700+09:00","updated":"2025-08-19T10:46:22.830+09:00"}
---

# Case Study
``` dataview
TABLE file.mtime AS "수정일"
FROM #casestudy
SORT file.mtime DESC
```

# Acting
``` dataview
TABLE file.mtime AS "수정일"
FROM #acting
SORT file.mtime DESC
```

# EMR 
``` dataview
TABLE file.mtime AS "수정일"
FROM #emr
SORT file.mtime DESC
```