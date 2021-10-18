# APK API Interface

APK Management
(/api-v1/apk)

- /add

To Add a apk.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 应用名 | appName | string | yes | |
| 上传者 | uploadedBy | string | yes | |

---

- /get-total

Get the total number of apks (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get apk list (Used for paging).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 页码号 | pageNumber | int | yes | |
| 分页大小 | pageSize | int | yes | |

---

- /get

Find the specific apk(s).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 应用名 | appName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |

---

- /is-exist

Determine whether the apk exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 应用名 | appName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | | 

---

- /delete

Delete the specific apk(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 应用名 | appName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |

---

- /update

Update the specific apk.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | yes | 
| 应用名 | appName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |

---