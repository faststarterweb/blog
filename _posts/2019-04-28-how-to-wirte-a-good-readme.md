---
title: How to Write a Good Readme
author: Cheney Zhang
date: 2024-07-15
category: start-up
layout: post
---
> Source : https://developer.aliyun.com/article/1468522

## Introduction

A complete README.md typically includes project title, description, installation guide, usage examples, contribution guide, license, and other sections. Each section is designed to provide readers with a more comprehensive and in-depth understanding of the project.
> 一个完整的 README.md 通常包括项目标题、描述、安装指南、使用示例、贡献指南、许可证等部分。每一部分都是为了让读者更全面、深入地了解项目。

### Project Title and Description
The title and description of the project are the core parts of the README, which succinctly and clearly convey the main purpose and functionality of the project. A good title can quickly capture the reader's attention, while a clear description can help readers understand the purpose and value of the project.
> 项目的标题和描述是 README 的核心部分，它简洁明了地传达了项目的主要目的和功能。一个好的标题能够快速吸引读者的注意力，而一个清晰的描述能够帮助读者理解项目的用途和价值。

### Installation Guide and Usage Examples
This section provides detailed steps to guide readers on how to install and use the project. It should include all necessary commands, scripts, and other relevant information to ensure that readers can run and use the project smoothly.
> 这一部分提供了详细的步骤，指导读者如何安装和使用项目。它应该包括所有必要的命令、脚本和其他相关信息，以确保读者能够顺利地运行和使用项目。

## Project Title and Description
In open source projects, an attractive title and clear description are crucial. It is not only the first impression of the project, but also a key factor determining whether people continue to read and explore.
> 在开源项目中，一个吸引人的标题和清晰的描述是至关重要的。它不仅是项目的第一印象，也是决定人们是否继续阅读和探索的关键因素。

### How to Choose an Attractive Title
A good title should be **concise, clear, and attractive**. It needs to accurately convey the main functions or features of the project while stimulating readers' interest and curiosity.
> 一个好的标题应该是简洁、明确和具有吸引力的。它需要准确地传达项目的主要功能或特点，同时激发读者的兴趣和好奇心。

For example, the project title of an audio and video player can be "UltraPlayer: Super Audio and Video Experience". As stated in 'Code Complete', 'Good code is self explanatory.' A good title should also be self explanatory, able to quickly tell readers what the project is about.
> 例如，一个音视频播放器的项目标题可以是“UltraPlayer：超级音视频体验”。“正如《代码大全》中所说：‘好的代码是自解释的。’” 一个好的标题也应该是自解释的，能够快速告诉读者这个项目是关于什么的。

| Feature | Good Title | Bad Title |
|---|---|---|
| Concise | UltraPlayer | A Liunx based Audio and Video Player |
| Clear | FastAPI Quickstart | API Project |
| Attractive| VisualizeDS: visualization of Data Structures | Data Structures Project | 

### Writing a Concise and Clear Project Description
Project description is an extension and supplement to the title, providing more details about the project. A good project description should be **concise and clear**, but also **detailed enough to help readers quickly understand the purpose**, functionality, and advantages of the project.
> 项目描述是对标题的扩展和补充，它提供了关于项目的更多细节。一个好的项目描述应该简洁明了，但也足够详细，能够帮助读者快速理解项目的用途、功能和优势。

For example, a description of a C++API library could be: "C++Master is an efficient and flexible C++API library designed to help developers quickly build stable and high-performance applications." Here, we clarify the project name, main features, and target audience.
> 例如，一个C++ API库的描述可以是：“C++Master是一个高效、灵活的C++ API库，旨在帮助开发者快速构建稳定和高性能的应用程序。” 在这里，我们明确了项目的名称、主要特点和目标受众。

#### Key Elements of Description
- **Conciseness :** Keep the description concise and avoid redundant and complex terminology
- **Clarity :** Clearly articulate the main functions and advantages of the project
- **Specificity :** Provide specific examples and purposes to help readers better understand the project
> - 简洁性 : 保持描述简洁，避免冗余和复杂的术语。
> - 明确性 : 清晰地表达项目的主要功能和优势。
> - 具体性 : 提供具体的例子和用途，帮助读者更好地理解项目。

### Installation and Usage Instructions
In open source projects, clear and concise installation and usage instructions are crucial. It not only helps users quickly understand how to get started, but also reduces the confusion and frustration they may encounter during installation and use.
> 在开源项目中，一个清晰、简洁的安装和使用说明是至关重要的。它不仅帮助用户快速理解如何开始，也减少了他们在安装和使用过程中可能遇到的困惑和挫败感。

#### Providing Detailed Installation Steps
Firstly, we need to provide a detailed step-by-step explanation to enable users to easily install and configure the project. For example, if your project is an audio and video player, you can follow these steps:
> 首先，我们需要提供一个详细的步骤说明，让用户能够轻松地安装和配置项目。例如，如果你的项目是一个音视频播放器，你可以按照以下步骤进行：

##### Clone the Repository
Users need to clone projects from GitHub or other code hosting platforms to their local environment. Specific command-line instructions can be provided, such as:
> 用户需要从GitHub或其他代码托管平台克隆项目到本地。可以提供具体的命令行指令，如：
```
git clone https://github.com/yourusername/yourprojectname.git
```

##### Install Dependencies
List all the dependencies required for the project and provide specific commands for installing these dependencies. For example:
> 列出项目所需的所有依赖，并提供安装这些依赖的具体命令。例如：
```
cd yourprojectname
sudo apt install <dependencies>
```

##### Compile the Project
Provide specific steps and commands for compiling the project. For example:
> 提供编译项目的具体步骤和命令。例如：
```
make
```
As stated in "C++Programming Ideas", The clarity of code is the foundation of excellent software.
> 正如《C++编程思想》中所说：“代码的清晰是优秀软件的基石。” 

#### How Users Can Use Your Project
In this section, we need to provide a detailed explanation of how to use the project, which can help users understand by providing specific usage scenarios and examples.
> 在这一部分，我们需要详细说明如何使用项目，可以通过提供具体的使用场景和示例来帮助用户理解。

For example, if your project is a C++API library, you can provide a simple example code that shows how to reference and use this library. Here, we can use tables to summarize and compare different usage scenarios.
> 例如，如果你的项目是一个C++ API库，你可以提供一个简单的示例代码，展示如何引用和使用这个库。在这里，我们可以使用表格来总结和对比不同的使用场景。

| Usage Scenarios | Sample Code | Description |
| --- | --- | --- |
| Reference Library | ``#include <yourlibrary>`` | This line of code demonstrates how to reference your library in a project |
| Call Function | ``yourFunction()`` | This is an example of calling a function in a library |

Here, we can quote a sentence from "Code Complete": "Code is meant for people to see, but it happens that machines can also execute it." This means that the code and documentation we write are primarily for the convenience of other developers to read and understand.
> 在这里，我们可以引用《代码大全》中的一句话：“代码是给人看的，只是恰好机器也能执行。” 这意味着我们写的代码和文档，首先是为了方便其他开发者阅读和理解。

#### Providing Help and Support
Finally, we need to provide a channel for users to receive help and support when they encounter problems. This can be a problem tracking system, a community forum, or a real-time chat room.
For example:
- **GitHub Issues** 
- **Community Forum** 
- **Live Chat** 

> 最后，我们需要提供一个渠道，让用户在遇到问题时能够获得帮助和支持。这可以是一个问题追踪系统、一个社区论坛或者一个实时聊天室。

In this section, we can quote Donald Knuth's famous quote in "The Art of Computer Programming": "Programs are written and read by humans, not executed by machines." This emphasizes that when writing code and documentation, we should always consider the human factor to make it easy to understand and use.
> 在这一部分，我们可以引用Donald Knuth在《计算机程序设计艺术》中的名言：“程序是为人类读写的，不是为机器执行的。” 这强调了我们在编写代码和文档时，应该始终考虑到人的因素，使其易于理解和使用。