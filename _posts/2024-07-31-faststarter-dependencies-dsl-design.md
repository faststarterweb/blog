---
title: FastStarter Dependencies DSL Design
author: Cheney Zhang
date: 2024-07-31
category: start-up
layout: post
---

## DSL Template

```black
{
    "dependency-key": { // dependency unique value
        "title": "", // dependencies-list-show-title
        "description": "", // dependencies-list-show-description
        "latest-version": "",
        "tip": "", // dependency tip message
        "versions": [ // all version list
            "1.xx": { // specific version number
                "tip":"", // version tips message
                "maven": {
                    "groupId":"",
                    "artifactId":"",
                    "scope":""
                },
                "gradle": "" // unsupported, leave as extension
            }
        ]

    }
}

```