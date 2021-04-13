Go AWS Lambda Builder Action
========================

GitHub action for building Go based lambdas

```yaml
- uses: aig787/go-lambda-builder@v1.0
  with:
    files: "main.go other/helper.go"
    credentials: ${{ secrets.GIT_CREDENTIALS }}
```
### Inputs
| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| files     | Source files to be built and packaged (space separated) | true | | 
| directory | Relative path under $GITHUB_WORKSPACE where source code is located | false |
| credentials | If provided git will be configured to use these credentials and https | false | |
