
- Copy the generated aar file and paste to the distribute repository
- Rename the SDK file as below format:
```
vietmap-tracking-sdk.version.aar
```
Example:
```
vietmap-tracking-sdk-1.1.0.aar
```
- Change the version in `jitpack.yml` file as below
```yml
 - FILE="-Dfile=vietmap-tracking-sdk.version.aar" 
 ```
- Create new tag __match with the version was created__
## The tag must be compliance with below format:
```yml
    [0-9]+.[0-9]+.[0-9]
i.e:
    1.0.1
```

- Commit and push new code to created tag
- Github action will release new version to jitpack automatically

## Clean project
- Build android SDK will created many large file, you should clean them after build success and release new version
- Use below command in the project terminal to clean unnecessary file in project
```bash
    make clean
```

### Go to https://jitpack.io/#vietmap-company/vietmap-tracking-sdk
and make sure the get it button of latest version is full-fill green status. If it getting white status, click it.