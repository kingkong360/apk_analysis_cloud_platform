# Report API Interface

Report Management
(/api-v1/report)

- /add

To Add a report.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 报告名称 | reportName | string | yes | Report name uses apk name + report + timestamp |
| 上传者 | uploadedBy | string | yes | |
| 应用名 | appName | string | yes | Which app is the report recorded |

---

- /get-total

Get the total number of reports (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get report list (Used for paging).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 页码号 | pageNumber | int | yes | |
| 分页大小 | pageSize | int | yes | |

---

- /get

Find the specific report(s).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 报告名称 | reportName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /is-exist

Determine whether the report exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 报告名称 | reportName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /delete

Delete the specific report(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 报告名称 | reportName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /update

Update the specific report.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | yes | 
| 报告名称 | reportName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---