# 🤖 CI Action

#### A simple action to build a WindowsAppSdk app.

---

## 🔤 Inputs

### `project-path`

**Optional** Path to the project file. Won't build the project if `project-path` is null.

### `test-project-path`

**Optional** Path to the test project file. Won't run tests if `test-project-path` is null.

### `timeout`

**Optional** Timeout minutes of the CI. Default is `60`.

## ⚡ Example Usage

```yaml
jobs:
  build_and_test:
    runs-on: windows-latest
    steps:
      - name: Run CI Action
        uses: Lamparter/Build-WinAppSdk@latest
        with:
          project-path: './src/FluentHub.App/FluentHub.App.csproj'
          test-project-path: './src/FluentHub.Tests/FluentHub.Tests.csproj'
          timeout: 15
```
