# 📊 Kestra Issue #6180
## [Overview](https://github.com/kestra-io/kestra/issues/6180)
- **Problem**: There is an unnecessary background behind the Search Input text.
- **Discussion**: Someone else had been assigned to the issue, but no PRs have been created yet. I came up with my own solution in [Week 13](https://github.com/bennColl-cs4387/camisola/blob/main/Solo%20Fixes/SOLO_PROGRESS4.md).

## Code
- `ui/src/styles/layout/element-plus-overload.scss` This file contains styling rules for the element's class, so I separated the `background-color` and `width` properties to get rid of the unnecessary background while maintaining the container dimensions for the Search bar.
```
.el-input, .el-input-number, .el-select, .el-date-editor.el-input {
    background-color: var(--bs-body-bg);
}

.el-input-number, .el-select, .el-date-editor.el-input {
    width: 100%;
}
```
