# Solo Fix Progress Report 2

## 🖼️ p5.JS Web Editor Issue #1852

### [Overview](https://github.com/processing/p5.js-web-editor/issues/1852)
- **Problem**: Text on the preview window is difficult to see when the user is in Dark or High Contrast mode.
- **Discussion**: Others have shared their fix attempts, but nothing has been merged yet; the project maintainers have been looking for the most appropriate fix user experience-wise.

### Progress
- **Code + Next Steps**: I found in `client/modules/IDE/actions/preferences.js` the main function for toggling between Light, Dark, and High Contrast modes, so I added a portion that modifies the (text) color based on the currently selected mode.
```
state.files.forEach((e) => {
      if (e.name === 'style.css' && state.preferences.theme !== 'light') {
        const regex = /color\s*:[^;]+;/g;
        e.content = e.content.replace(regex, 'color: white;');
      }
    })
```
- I need to continue looking through and modifying the style.css and other `client/modules/IDE` files to make sure the preview window itself updates accordingly when the `play-button` is active.
