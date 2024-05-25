---
title: Roadmap
draft: false
tags:
  - technical
date:
---

### Upcoming


### Working
- Newsletter collections


### Shipped
- guide folder 2024-05-25
- booknotes folder 2024-05-24
- Rules Page 2024-05-12
- Newsletter Page 2024-05-05
- Roadmap Page 2024-05-02
- quartz.config.ts grey style 2024-05-02
- Custom Domain 2024-05-01
- Reminders Page 2024-03-10
- Books Page 2024-03-10
- Home Page 2024-03-10
- About Page 2024-03-10
- Now Page 2024-03-09



---

#### Website Building Braindump
1. **[[the why of this blog|The Why of This Blog]]**
	1. serve my mind and brain
	2. build the portal to meet people
	3. share life with friends
2. **publish easily**
	1. random thoughts / questions
	2. newsletter
	3. reading notes
3. **stay minimal**
	1. [Jacky Zhao](https://jzhao.xyz/) (Quartz)
	2. [Steph Ango](https://stephango.com/) (Obsidian)
	3. [Cheng-Wei Hu](https://chengweihu.com/) 
4. **like-minded reference** 
	1. [Derek Sivers](https://sive.rs/) 
	2. [David Perell.](https://perell.com/) (WordPress)
	3. [PJ Wu](https://pinchlime.com/) (Zola)
	4. [Bryan Jenks](https://www.bryanjenks.dev/) (Squarespace)
	5. [Owen Young](https://www.owenyoung.com/) (Zola)
	6. [Joel Gascoigne](https://joel.is/) (Ghost)
	7. [Matt D'Avella](https://www.mattdavella.com/) (Squarspace)
	8. [Craig Mod](https://craigmod.com/)
	9. [Tim Ferriss](https://tim.blog/) (WordPress)
	10. [Eyewithouts](https://eyewithouts.com/)
5. **ideal update frequency**
	1. daily update - homework for life
	2. weekly update - newsletter
	3. monthly update - book notes / mini presentation / project update

---

## Changelog

#### [1.1.1] - 2024-05-02

##### modified

- [Typescript] Remove all the dates

``` css
// components for pages that display a single page (e.g. a single note)
export const defaultContentPageLayout: PageLayout = {
  beforeBody: [
    Component.ContentMeta(), // ← remove this line //
  ],
```

#### [1.0.1] - 2024-05-02

##### modified

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

#### [1.0.0] - 2024-05-01

##### checked

1. Prepare Obsidian vault
2. Download and install Quartz
3. Create GitHub repository 
4. Sync to GitHub
5. Deploy to Cloudflare