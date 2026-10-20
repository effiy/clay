---
title: "GLES3 Renderer Scrolling Container (SDL2)"
tags: [clay, gles3, sdl2, renderer, sidebar, scrolling]
category: "example"
created: 2026-10-20
source: "https://github.com/nicbarker/clay"
type: demo
status: work-in-progress
description: "Clay GLES3 renderer sidebar scrolling container example using SDL2, demonstrating all draw commands."
---

# GLES3 Renderer Scrolling Container (Using SDL2)

This directory contains a complete example that can be used to test all different draw commands using work-in-progress GLES3 renderer. While it still needs refinement, the renderer is already functional and demonstrates the core rendering pipeline.

---

## 💡 概述

完整的示例，可用于测试所有不同的绘制命令。使用开发中的 GLES3 渲染器，虽然仍需改进但已可用。

The images used as resources in this example, namely:

- millbank.jpeg a window with a panoramic city view;
- and profile-picture.png showing objects aligned in a circle;

are taken with my phone camera and are dedicated to the Public Domain.

---

## ⚡ 功能

- 测试所有不同的绘制命令
- GLES3 渲染器核心渲染管线演示
- 边栏滚动容器布局

---

## 📊 指标

「待补充」

---

## 🏛️ 设计

「待补充」

---

## 📁 目录

「待补充」

---

## 🔗 资源

「待补充」

---

## 🚀 快速开始

### How to build it with CMake?

Cmake build is the easiest way to build it:

    mkdir build
    cmake -S . -B ./build

### How to build and run on Emscripten:

For Emscripten the build is a bit custom, but it depends on CMakeBuild to install header-stb dependency. So you still need to build it with CMake first.

And then you have to source the Emscripten SDK:

    source /path/to/emscripten/emsdk/emsdk_env.sh

Then build it with hand-crafted Makefile.emscripten:

    make -f Makefile.emscripten test

and then navigate to http://localhost:8080

### How to build and run on Mac:

Requires SDL2:

    brew install sdl2

Requires STB:

    cmake -B build

Build it with:

    make -f Makefile.macos

And run with:

    ./macos-sidebar-scrolling-container-sdl2

---

## ⚙️ 技术栈

- GLES3
- SDL2
- C / C++
- stb_image.h / stb_truetype.h
- Emscripten
- CMake