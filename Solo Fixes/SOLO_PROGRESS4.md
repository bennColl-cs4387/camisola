# Solo Fix Progress Report 4

## 📊 Kestra Frontend Issues

### [Overview](https://github.com/kestra-io/kestra/issues)
- **Overview**: Kestra has several open issues labeled _good first issue_. I decided to tackle some of these frontend issues for the rest of my solo fixes.
- **Discussion**: Most of these issues have already been assigned to others, but no PRs have been made nor merged.

### Progress
- **Building Codebase**: Before anything else, I built the codebase to work without the backend. This was done with `Docker`.
```
$ docker-compose up
$ cd ui
$ nano .env.development.local
$ npm install
$ npm run dev
```
- **Issue 6180 ✅**: In `ui/src/styles/layout/element-plus-overload.scss`, I separated the `background-color` and `width` properties to get rid of the unnecessary background while  maintaining the container dimensions for the Search bar.
```
.el-input, .el-input-number, .el-select, .el-date-editor.el-input {
    background-color: var(--bs-body-bg);
}

.el-input-number, .el-select, .el-date-editor.el-input {
    width: 100%;
}
```
