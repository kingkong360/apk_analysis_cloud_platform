# Video API Interface

Video Management
(/api-v1/video)

- /add

To Add a video.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 视频名称 | videoName | string | yes | Video name uses apk name + report + timestamp |
| 上传者 | uploadedBy | string | yes | |
| 应用名 | appName | string | yes | Which app is the video recorded |

---

- /get-total

Get the total number of videos (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get video list (Used for paging).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 页码号 | pageNumber | int | yes | |
| 分页大小 | pageSize | int | yes | |

---

- /get

Find the specific video(s).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 视频名称 | videoName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /is-exist

Determine whether the video exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 视频名称 | videoName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /delete

Delete the specific video(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | Optional | 
| 视频名称 | videoName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---

- /update

Update the specific video.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | id | int | yes | 
| 视频名称 | videoName | string | Optional | |
| 上传者 | uploadedBy | string | Optional | |
| 应用名 | appName | string | Optional | |

---