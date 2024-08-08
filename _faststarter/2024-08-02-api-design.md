---
title: Design - API
author: Cheney Zhang
date: 2024-08-02
category: faststarter
layout: post
---

## 1. Parameter Template
### 1.1 Request Template
```black
{
    "sign":"" // request signature, backend verification of whether the request is legitimate
}
```
### 1.2 Response Template
```black
{
    "code":"",
    "error":"",
    "errorMessage":"",
    "data" : {} // data returned after successful request
}
```

## 2. APIs
### 2.1 Get Dependencies

| **Method** | **URL** | 
| --- | --- |
| GET | ``/faststarter/dependencies`` |

#### 2.1.1 Request

| **Parameter** | **Description** |
| --- | --- |
| sign | request signature, backend verification of whether the request is legitimate |

#### 2.1.2 Response
```black
{
    ---
    "data": [
        {
            "dependencyKey" : "",
            "title" : "",
            "description" : "",
            "category" : "",
            "tip" : ""
        }
    ]
}
```

### 2.2 Generate

| **Method** | **URL** |
| --- | --- |
| POST | ``/faststarter/generate`` |

#### 2.2.1 Request
```black
{
    "language" : "java",
    "project" : "maven",
    "style" : "",
    "springBootVersion" : "",
    "projectMetadata" : {
        "group" : ""
        "artifact" : ""
        "name" : ""
        "description" : ""
        "packageName" : ""
        "packaging" : ""
        "javaVersion" : ""
    },
    "dependencies":[""],
    "sign":"" // request signature, backend verification of whether the request is legitimate
}
```

#### 2.2.2 Response
```black
{
    ---
    "data" : {
        "downloadUrl":"" // frontend download file througth the downloadUrl
    }
}
```