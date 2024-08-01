---
title: FastStarter Dependency DSL Design
author: Cheney Zhang
date: 2024-07-31
category: start-up
layout: post
---

## DSL Template

```black
{
    "`dependency-key`": {
        "title": "",
        "description": "",
        "latest-version": "",
        "tags": [],
        "categories": "",
        "versions": {
            "`1.xx`": {
                "tip":"",
                "maven": {
                    "groupId":"",
                    "artifactId":"",
                    "scope":""
                }
            }
        }
    }
}

```

## Feild Description
- **`dependency-key` :** used to determine a denpdency, when using, it needs to be replaced with a user-defined key
-  **title :** the title displayed on the dependency list page in the frontend
-  **latest-version :** the lastest version of the current dependency
-  **tags :** dependency tags
-  **categories :** dependency categories
-  **versions :**  details of each version of the dependency
-  **`1.xx` :** specific version number, when using, it needs to be replaced with a real version number
-  **tip :** version tips message
-  **maven :** maven configuration

## Example
### Spring Boot
```black
{
    "springboot": {
        "title": "SpringBoot",
        "description": "Buession Framework Springboot Boot",
        "latest-version": "2.3.3",
        "tags": ["spring"],
        "categories": "springboot",
        "versions": {
            "2.3.3": {
                "tip":"Vulnerabilities:CVE-2022-1471",
                "maven": {
                    "groupId":"com.buession.springboot",
                    "artifactId":"buession-springboot-boot"
                }
            },
            "2.3.2": {
                "tip":"Vulnerabilities:CVE-2022-1471",
                "maven": {
                    "groupId":"com.buession.springboot",
                    "artifactId":"buession-springboot-boot"
                }
            }
        }
    }
}
```
### Spring Boot Starter Web
```black
{
    "spring-boot-starter-web": {
        "title": "Spring-Boot-Starter-Web",
        "description": "Starter for building web, including RESTful, applications using Spring MVC. Uses Tomcat as the default embedded container",
        "latest-version": "2.3.3",
        "tags": ["spring","framework","web","starter"],
        "categories": "web-frameworks",
        "versions": {
            "3.3.2": {
                "tip":"",
                "maven": {
                    "groupId":"org.springframework.boot",
                    "artifactId":"spring-boot-starter-web"
                }
            },
            "3.3.1": {
                "tip":"",
                "maven": {
                    "groupId":"org.springframework.boot",
                    "artifactId":"spring-boot-starter-web"
                }
            }
        }
    }
}
```
### Jackson Core
```black
{
    "jackson-core": {
        "title": "Jackson-Core",
        "description": "Core Jackson processing abstractions (aka Streaming API), implementation for JSON",
        "latest-version": "2.17.2",
        "tags": [
            "format",
            "json",
            "serialization",
            "jackson"
        ],
        "categories": ["json-libraries"],
        "versions": {
            "2.17.2": {
                "maven": {
                    "groupId":"com.fasterxml.jackson.core",
                    "artifactId":"jackson-core"
                }
            },
            "2.17.1": {
                "maven": {
                    "groupId":"com.fasterxml.jackson.core",
                    "artifactId":"jackson-core"
                }
            }
        }
    }
}
```
### Integrated configuration
```black
{
    "springboot": {
        "title": "SpringBoot",
        "description": "Buession Framework Springboot Boot",
        "latest-version": "2.3.3",
        "tags": ["spring"],
        "categories": "springboot",
        "versions": {
            "2.3.3": {
                "tip":"Vulnerabilities:CVE-2022-1471",
                "maven": {
                    "groupId":"com.buession.springboot",
                    "artifactId":"buession-springboot-boot"
                }
            },
            "2.3.2": {
                "tip":"Vulnerabilities:CVE-2022-1471",
                "maven": {
                    "groupId":"com.buession.springboot",
                    "artifactId":"buession-springboot-boot"
                }
            }
        }
    },
    "spring-boot-starter-web": {
        "title": "Spring-Boot-Starter-Web",
        "description": "Starter for building web, including RESTful, applications using Spring MVC. Uses Tomcat as the default embedded container",
        "latest-version": "2.3.3",
        "tags": ["spring","framework","web","starter"],
        "categories": "web-frameworks",
        "versions": {
            "3.3.2": {
                "tip":"",
                "maven": {
                    "groupId":"org.springframework.boot",
                    "artifactId":"spring-boot-starter-web"
                }
            },
            "3.3.1": {
                "tip":"",
                "maven": {
                    "groupId":"org.springframework.boot",
                    "artifactId":"spring-boot-starter-web"
                }
            }
        }
    },
    "jackson-core": {
        "title": "Jackson-Core",
        "description": "Core Jackson processing abstractions (aka Streaming API), implementation for JSON",
        "latest-version": "2.17.2",
        "tags": [
            "format",
            "json",
            "serialization",
            "jackson"
        ],
        "categories": ["json-libraries"],
        "versions": {
            "2.17.2": {
                "maven": {
                    "groupId":"com.fasterxml.jackson.core",
                    "artifactId":"jackson-core"
                }
            },
            "2.17.1": {
                "maven": {
                    "groupId":"com.fasterxml.jackson.core",
                    "artifactId":"jackson-core"
                }
            }
        }
    }
}
```