# Solo Fix Progress Report 1

## 🖼️ p5.JS Web Editor Issue #1852

### [Overview](https://github.com/processing/p5.js-web-editor/issues/1852)
- **Problem**: Text on the preview window is difficult to see when the user is in Dark or High Contrast mode.
- **Discussion**: Others have shared their fix attempts, but nothing has been merged yet; the project maintainers have been looking for the most appropriate fix user experience-wise.

### Progress
- **Building Codebase**: I built the codebase back in Week 5, so doing this again was almost straightforward. In addition to the instructions in the Contributor Guidelines, I also had to install & update additional scrips such as nvm.
- **Bug Replication**: Running it on my local host, I was able to reproduce the issue as directed in the original Issue report. I also experimented with reproducing the same bug in different use cases.
- **Analysis**: I looked through the codebase's files to better understand the issue and plan out my solution. Moreover, I looked through the previous pull requests to test out their attempts.
- **Code + Next Steps**: I was able to experiment with switching styles/colors when toggling between accessibility modes to improve legibility, but this is similar to the old pull requests that weren't merged — I still need to work on the override rules and come up with a more thoughtful solution.


## 🌐 Pixijs Issue #10162

### [Overview](https://github.com/pixijs/pixijs/issues/10162)
- **Problem**: The background color of a sketch is unchangeable if initialized with an opaque background.
- **Discussion**: A lead maintainer says that the "alpha" value is only used in initialization.

### Progress
- **Research & Understanding**: I am completely new to this codebase, so I spent time looking through the project and its Community Guidelines to understand how I could contribute.
- **Building Codebase**: There were two ways of building the environment, so I tried doing both — this also took a while.
