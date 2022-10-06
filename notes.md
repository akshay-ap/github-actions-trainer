# Study notes
- GIthub actions is about automating development process workflow
- Github actions require some naming conventions of directory and subdirectory
  - `.github/workflows`
- Event, jobs, ..etc
- Show status turning green or red
- Event example
```yml
on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]
```
- Each job runs on a separate server - by default jobs run in parallel
 - if you want job to run after another job then use `needs: name_of_job`
```yaml
jobs:
  build:
  publish:
    needs: build
```
# TODO:
- Run my own simple hardhat project with mvp github actions
- Find resources