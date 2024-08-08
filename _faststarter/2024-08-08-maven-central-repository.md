---
title: Design - Maven Central Repository
author: Cheney Zhang
date: 2024-08-08
category: faststarter
layout: post
---

## Maven Central Repository

To better utilize maven central repository, integrate the search API of maven central repository.

## Maven Central Repository REST API

> These URLs allow you to access the search functionality of the Central Repository from any non-browser user agent. Note that the "wt" param- eter present in every URL determines the format of the results. Setting "wt" equal to "json" will provide a JSON response, while setting "wt" equal to "xml" will provide the same response formatted as an XML document. Another common parameter is "rows," which limits the number of results returned by the server.

| Order | URL | Description |
| - | --- | --- |
| `1` | ``https://search.maven.org/solrsearch/select?q=guice&rows=20&wt=json`` | Mimics typing "guice" in the basic search box. Returns first page of artifacts with "guice" in the groupId or artifactId and lists details for most recent version released. |
| `2` | ``https://search.maven.org/solrsearch/select?q=g:com.google.inject+AND+a:guice&core=gav&rows=20&wt=json`` | Mimics clicking the link for all versions of groupId "com.google.inject" and artifactId "guice." Returns sorted list of all versions of an artifact. |

## URL `1`
```black
{
    "responseHeader": {
        "status": 0,
        "QTime": 16,
        "params": {
            "q": "tags:scalaVersion-2.9",
            "core": "",
            "indent": "off",
            "spellcheck": "true",
            "fl": "id,g,a,latestVersion,p,ec,repositoryId,text,timestamp,versionCount",
            "start": "",
            "spellcheck.count": "5",
            "sort": "score desc,timestamp desc,g asc,a asc",
            "rows": "20",
            "wt": "json",
            "version": "2.2"
        }
    },
    "response": {
        "numFound": 263,
        "start": 0,
        "docs": [
            {
                "id": "net.koofr:sbt-jaxws-1734730745",
                "g": "net.koofr",
                "a": "sbt-jaxws",
                "latestVersion": "0.2",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1437046609000,
                "versionCount": 2,
                "text": [
                    "net.koofr",
                    "sbt-jaxws",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-dependency-graph-1734730745",
                "g": "net.virtual-void",
                "a": "sbt-dependency-graph",
                "latestVersion": "0.7.5",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1427695888000,
                "versionCount": 10,
                "text": [
                    "net.virtual-void",
                    "sbt-dependency-graph",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-dependency-graph327821292",
                "g": "net.virtual-void",
                "a": "sbt-dependency-graph",
                "latestVersion": "0.7.5",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1427695876000,
                "versionCount": 11,
                "text": [
                    "net.virtual-void",
                    "sbt-dependency-graph",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-dependency-graph116470379",
                "g": "net.virtual-void",
                "a": "sbt-dependency-graph",
                "latestVersion": "0.7.5",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1427695868000,
                "versionCount": 11,
                "text": [
                    "net.virtual-void",
                    "sbt-dependency-graph",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-dependency-graph-94880534",
                "g": "net.virtual-void",
                "a": "sbt-dependency-graph",
                "latestVersion": "0.7.5",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1427695857000,
                "versionCount": 11,
                "text": [
                    "net.virtual-void",
                    "sbt-dependency-graph",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.foursquare:spindle-codegen-plugin-1734730745",
                "g": "com.foursquare",
                "a": "spindle-codegen-plugin",
                "latestVersion": "3.0.0-M7",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1423076758000,
                "versionCount": 45,
                "text": [
                    "com.foursquare",
                    "spindle-codegen-plugin",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.foursquare:spindle-codegen-plugin-1734730776",
                "g": "com.foursquare",
                "a": "spindle-codegen-plugin",
                "latestVersion": "3.0.0-M6.1",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1418839599000,
                "versionCount": 43,
                "text": [
                    "com.foursquare",
                    "spindle-codegen-plugin",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-boilerplate-1734730745",
                "g": "net.virtual-void",
                "a": "sbt-boilerplate",
                "latestVersion": "0.5.9",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1409649583000,
                "versionCount": 1,
                "text": [
                    "net.virtual-void",
                    "sbt-boilerplate",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-boilerplate327821292",
                "g": "net.virtual-void",
                "a": "sbt-boilerplate",
                "latestVersion": "0.5.9",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1409649562000,
                "versionCount": 1,
                "text": [
                    "net.virtual-void",
                    "sbt-boilerplate",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "net.virtual-void:sbt-boilerplate116470379",
                "g": "net.virtual-void",
                "a": "sbt-boilerplate",
                "latestVersion": "0.5.9",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1409649547000,
                "versionCount": 1,
                "text": [
                    "net.virtual-void",
                    "sbt-boilerplate",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "info.schleichardt:sbt-sonar-1734730745",
                "g": "info.schleichardt",
                "a": "sbt-sonar",
                "latestVersion": "0.2.0",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1406696215000,
                "versionCount": 1,
                "text": [
                    "info.schleichardt",
                    "sbt-sonar",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "info.schleichardt:sbt-sonar327821292",
                "g": "info.schleichardt",
                "a": "sbt-sonar",
                "latestVersion": "0.2.0",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1406696205000,
                "versionCount": 1,
                "text": [
                    "info.schleichardt",
                    "sbt-sonar",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.gilt:sbt-dependency-graph-sugar-1734730745",
                "g": "com.gilt",
                "a": "sbt-dependency-graph-sugar",
                "latestVersion": "0.7.4",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1402152396000,
                "versionCount": 1,
                "text": [
                    "com.gilt",
                    "sbt-dependency-graph-sugar",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "pl.morgaroth:sbt-clearer-1734730745",
                "g": "pl.morgaroth",
                "a": "sbt-clearer",
                "latestVersion": "0.1.0",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1401402741000,
                "versionCount": 1,
                "text": [
                    "pl.morgaroth",
                    "sbt-clearer",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.twitter:scrooge-sbt-plugin-1734730745",
                "g": "com.twitter",
                "a": "scrooge-sbt-plugin",
                "latestVersion": "3.14.1",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1398970502000,
                "versionCount": 31,
                "text": [
                    "com.twitter",
                    "scrooge-sbt-plugin",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.github.dzsessona:sbt-neo-dependencies-1734730745",
                "g": "com.github.dzsessona",
                "a": "sbt-neo-dependencies",
                "latestVersion": "1.1.0",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1396471598000,
                "versionCount": 3,
                "text": [
                    "com.github.dzsessona",
                    "sbt-neo-dependencies",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.atlassian.labs:sbt-git-stamp-1734730745",
                "g": "com.atlassian.labs",
                "a": "sbt-git-stamp",
                "latestVersion": "0.1.2",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1396462843000,
                "versionCount": 1,
                "text": [
                    "com.atlassian.labs",
                    "sbt-git-stamp",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.atlassian.labs:sbt-git-stamp327821292",
                "g": "com.atlassian.labs",
                "a": "sbt-git-stamp",
                "latestVersion": "0.1.2",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1396462831000,
                "versionCount": 1,
                "text": [
                    "com.atlassian.labs",
                    "sbt-git-stamp",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.atlassian.labs:sbt-git-stamp116470379",
                "g": "com.atlassian.labs",
                "a": "sbt-git-stamp",
                "latestVersion": "0.1.2",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1396462823000,
                "versionCount": 1,
                "text": [
                    "com.atlassian.labs",
                    "sbt-git-stamp",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            },
            {
                "id": "com.github.dzsessona.sbt-neo-dependencies:sbt-neo-dependencies-1734730745",
                "g": "com.github.dzsessona.sbt-neo-dependencies",
                "a": "sbt-neo-dependencies",
                "latestVersion": "0.1.1",
                "repositoryId": "central",
                "p": "jar",
                "timestamp": 1395356537000,
                "versionCount": 1,
                "text": [
                    "com.github.dzsessona.sbt-neo-dependencies",
                    "sbt-neo-dependencies",
                    ".jar",
                    ".pom"
                ],
                "ec": [
                    ".jar",
                    ".pom"
                ]
            }
        ]
    },
    "spellcheck": {
        "suggestions": [
            "scalaversion",
            {
                "numFound": 5,
                "startOffset": 5,
                "endOffset": 19,
                "suggestion": [
                    "scmversion",
                    "javaversion",
                    "conversion",
                    "subversion",
                    "javersion"
                ]
            }
        ]
    }
}
```

## URL `2`

```black
{
    "responseHeader": {
        "status": 0,
        "QTime": 218,
        "params": {
            "q": "g:com.google.inject AND a:guice",
            "core": "gav",
            "indent": "off",
            "fl": "id,g,a,v,p,ec,timestamp,tags",
            "start": "",
            "sort": "score desc,timestamp desc,g asc,a asc,v desc",
            "rows": "20",
            "wt": "json",
            "version": "2.2"
        }
    },
    "response": {
        "numFound": 24,
        "start": 0,
        "docs": [
            {
                "id": "com.google.inject:guice:7.0.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "7.0.0",
                "p": "jar",
                "timestamp": 1683913265000,
                "ec": [
                    "-sources.jar",
                    ".pom",
                    "-test-sources.jar",
                    "-javadoc.jar",
                    "-tests.jar",
                    ".jar",
                    "-classes.jar"
                ],
                "tags": [
                    "framework",
                    "java",
                    "dependency",
                    "above",
                    "injection",
                    "guice",
                    "lightweight"
                ]
            },
            {
                "id": "com.google.inject:guice:6.0.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "6.0.0",
                "p": "jar",
                "timestamp": 1683912686000,
                "ec": [
                    "-sources.jar",
                    ".pom",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".jar"
                ],
                "tags": [
                    "framework",
                    "java",
                    "dependency",
                    "above",
                    "injection",
                    "guice",
                    "lightweight"
                ]
            },
            {
                "id": "com.google.inject:guice:6.0.0-rc2",
                "g": "com.google.inject",
                "a": "guice",
                "v": "6.0.0-rc2",
                "p": "jar",
                "timestamp": 1683237024000,
                "ec": [
                    "-sources.jar",
                    ".pom",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".jar"
                ],
                "tags": [
                    "framework",
                    "java",
                    "dependency",
                    "above",
                    "injection",
                    "guice",
                    "lightweight"
                ]
            },
            {
                "id": "com.google.inject:guice:7.0.0-rc1",
                "g": "com.google.inject",
                "a": "guice",
                "v": "7.0.0-rc1",
                "p": "jar",
                "timestamp": 1683235057000,
                "ec": [
                    "-sources.jar",
                    ".pom",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".jar"
                ],
                "tags": [
                    "framework",
                    "java",
                    "dependency",
                    "above",
                    "injection",
                    "guice",
                    "lightweight"
                ]
            },
            {
                "id": "com.google.inject:guice:6.0.0-rc1",
                "g": "com.google.inject",
                "a": "guice",
                "v": "6.0.0-rc1",
                "p": "jar",
                "timestamp": 1682631638000,
                "ec": [
                    "-sources.jar",
                    ".pom",
                    "-test-sources.jar",
                    "-javadoc.jar",
                    "-tests.jar",
                    ".jar",
                    "-classes.jar"
                ],
                "tags": [
                    "framework",
                    "java",
                    "dependency",
                    "above",
                    "injection",
                    "guice",
                    "lightweight"
                ]
            },
            {
                "id": "com.google.inject:guice:5.1.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "5.1.0",
                "p": "jar",
                "timestamp": 1643061977000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:5.0.1",
                "g": "com.google.inject",
                "a": "guice",
                "v": "5.0.1",
                "p": "jar",
                "timestamp": 1614380510000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:5.0.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "5.0.0",
                "p": "jar",
                "timestamp": 1614262656000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    ".jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:5.0.0-BETA-1",
                "g": "com.google.inject",
                "a": "guice",
                "v": "5.0.0-BETA-1",
                "p": "jar",
                "timestamp": 1603840959000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.2.3",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.2.3",
                "p": "jar",
                "timestamp": 1584647910000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    ".jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.2.2",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.2.2",
                "p": "jar",
                "timestamp": 1540834172000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.2.1",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.2.1",
                "p": "jar",
                "timestamp": 1537454300000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    ".jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.2.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.2.0",
                "p": "jar",
                "timestamp": 1519843925000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.1.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.1.0",
                "p": "jar",
                "timestamp": 1466193194000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.0",
                "p": "jar",
                "timestamp": 1430253206000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-site.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.0-beta5",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.0-beta5",
                "p": "jar",
                "timestamp": 1411592603000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    "-test-sources.jar",
                    "-tests.jar",
                    ".jar",
                    "-site.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.0-beta4",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.0-beta4",
                "p": "jar",
                "timestamp": 1395352292000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-site.jar",
                    "-no_aop.jar",
                    "-classes.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:4.0-beta",
                "g": "com.google.inject",
                "a": "guice",
                "v": "4.0-beta",
                "p": "jar",
                "timestamp": 1375308146000,
                "ec": [
                    "-sources.jar",
                    "-javadoc.jar",
                    "-test-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    "-no_deps.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:3.0",
                "g": "com.google.inject",
                "a": "guice",
                "v": "3.0",
                "p": "jar",
                "timestamp": 1301077187000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            },
            {
                "id": "com.google.inject:guice:3.0-rc3",
                "g": "com.google.inject",
                "a": "guice",
                "v": "3.0-rc3",
                "p": "jar",
                "timestamp": 1299460443000,
                "ec": [
                    "-javadoc.jar",
                    "-sources.jar",
                    ".jar",
                    "-tests.jar",
                    "-no_aop.jar",
                    ".pom"
                ],
                "tags": [
                    "dependency",
                    "guice",
                    "injection",
                    "above",
                    "java",
                    "lightweight",
                    "framework"
                ]
            }
        ]
    }
}
```