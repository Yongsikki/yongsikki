---
{"dg-publish":true,"permalink":"/case-study/nursing/","created":"2025-08-19T12:07:06.000+09:00","updated":"2025-09-30T15:53:06.828+09:00"}
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

