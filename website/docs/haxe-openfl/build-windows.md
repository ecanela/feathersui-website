---
title: Build a Feathers UI project as a Windows app
sidebar_label: Windows
---

[Feathers UI](/) may be used to build desktop applications targeting Microsoft's Windows operating system.

## Prerequisites

In addition to the dependencies specified in the [Feathers UI installation instructions](./installation.md), building a Windows application with Feathers UI has some additional requirements.

- A computer running Microsoft Windows. Windows apps cannot be built on other operating systems, such as macOS or Linux.
- Install [Visual Studio](https://visualstudio.microsoft.com/downloads/). The [Community edition](https://visualstudio.microsoft.com/vs/community/) is free.

## Build

To build for the `windows` target, run the following command.

```sh
openfl build windows
```

Use the `-debug` flag to create a build to include extra debugging information, including full stack traces when there's an exception or crash.

```sh
openfl build windows -debug
```

The build's output will be written to the _bin/windows/bin_ folder.

> Your [_project.xml_ file](https://lime.openfl.org/docs/project-files/xml-format/) may optionally specify an output folder different from _bin_.
>
> ```xml
> <app path="Export"/>
> ```
>
> In the example above, the output would be generated in _Export/windows/bin_ instead.

## Run / Debug

OpenFL provides the `test` command to compile and launch your project executable on Windows.

```sh
openfl test windows
```

## Troubleshooting

In the future, common error messages and their solutions will appear in this section.

> ### Did you get some other error message that you don't understand?
>
> Configuring OpenFL to build for native targets, like Windows or macOS, can be a little tricky! Head over to either the [Feathers UI community forum](https://community.feathersui.com/) or the [Feathers UI Discord](https://discord.feathersui.com/). Explain which command you tried to run, be sure to mention that you are targeting **windows**, and post the error message (and any additional relevant output). Ideally, we can help you figure out a solution, and then we'll also add it to this troubleshooting section, so that everyone can benefit.
