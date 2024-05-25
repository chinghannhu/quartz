---
title: Changelog
draft: false
tags:
  - technical
date: 2024/05/01
description:
---
## [1.1.1] - 2024-05-02

### modified

- [Typescript] Remove all the dates

``` css
// components for pages that display a single page (e.g. a single note)
export const defaultContentPageLayout: PageLayout = {
  beforeBody: [
    Component.ContentMeta(), // ← remove this line //
  ],
```

## [1.0.1] - 2024-05-02

### modified

- [Typescript] Color scheme

``` css
      colors: {
        lightMode: {
          light: "#fffcf3",
          lightgray: "#eeece6",
          gray: "#b8b8b8",
          darkgray: "#394047",
          dark: "#333438",
          secondary: "#1a1a1a",
          tertiary: "#737882",
          highlight: "#73788226",
        },
        darkMode: {
          light: "#222222",
          lightgray: "#333438",
          gray: "#505358",
          darkgray: "#dcdcdc",
          dark: "#dcdee1",
          secondary: "#9198a0",
          tertiary: "#a7adb3",
          highlight: "#dcdee126",
        },
```

## [1.0.0] - 2024-05-01

### checked

1. Prepare Obsidian vault
2. Download and install Quartz
3. Create GitHub repository 
4. Sync to GitHub
5. Deploy to Cloudflare