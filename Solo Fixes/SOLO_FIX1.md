# 🖼️ p5.JS Web Editor Issue #1852
## [Overview](https://github.com/processing/p5.js-web-editor/issues/1852)
- **Problem**: Text on the preview window is difficult to see when the user is in Dark or High Contrast mode.
- **Discussion**: Others have shared their fix attempts, but nothing has been merged yet; the project maintainers have been looking for the most appropriate fix user experience-wise.

## Code
- `client/modules/IDE/actions/preferences.js` This file contains the main function for toggling between Light, Dark, and High Contrast modes, so I added a portion that modifies the (text) color based on the currently selected mode.
```
state.files.forEach((e) => {
      if (e.name === 'style.css' && state.preferences.theme !== 'light') {
        const regex = /color\s*:[^;]+;/g;
        e.content = e.content.replace(regex, 'color: white;');
      }
    })
```
![Screenshot of Fix](https://github.com/bennColl-cs4387/camisola/blob/1556ea12994f09058fbf5968acde4bb7ef341535/Solo%20Fixes/p5.JS%20Web%20Editor%20-%20Issue%201852%20Fix.png)
