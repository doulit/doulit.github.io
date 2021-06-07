1. 모든 개발은 `develop` Branch를 기준으로 이루어진다.

   - 그러므로, `Main` Branch에 직접적인 commit을 할 경우는 존재하지 않는다.

2. 이슈에 대한 처리는 `develop` Branch를 기준으로 `feature/이슈번호/기능설명(영어로)` Branch를 개발자가 임의로 직접 생성하여 작업한다.

   - ex) feature/13/main/update

   ```Bash
    git checkout develop
    git pull develop
    git checkout -b `feature/이슈번호/기능설명(영어로)`
   ```

3. 해당 feature Branch에서의 작업을 다 끝내고 `git push` 까지 하였을 경우 `develop` Branch로 **Pull Request**를 올린다.
