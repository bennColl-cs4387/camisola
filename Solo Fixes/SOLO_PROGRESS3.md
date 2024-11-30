# Solo Fix Progress Report 3

## 🖼️ p5.JS Web Editor Issue #1852

### [Overview](https://github.com/processing/p5.js-web-editor/issues/1852)
- **Problem**: Text on the preview window is difficult to see when the user is in Dark or High Contrast mode.
- **Discussion**: Others have shared their fix attempts, but nothing has been merged yet; the project maintainers have been looking for the most appropriate fix user experience-wise.

### Progress
- **Code + Next Steps**: Referencing the other PRs, I had to implement the following to `client/modules/IDE/components/Editor/index.jsx` to have the changes reflected when refreshing. I anticipate that I should be finished with my solution by next week. 
```
componentWillUpdate(nextProps) {
    // check if files have changed
    if (this.props.files[0].id !== nextProps.files[3].id) {
      // files[0] changed to files[3]
```
