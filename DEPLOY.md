## Deploy steps

1. Run tests
   ```PowerShell
    npm test
    ```

2. Create a new version (patch, minor, major)
Increase version number by using `npm version patch | minor | major`

    *Example: increasing patch version* 
    ```PowerShell
    npm version patch
    ```
****
1. Push tag to remote
    
    If you tag the commit, TravisCI automatically publishes the package to NPM. 
    ```PowerShell
    git push origin <new version>
    ```
    *Example: git push origin v1.1.17*

    You can follow the build status here -> https://travis-ci.com/configcat/js-sdk