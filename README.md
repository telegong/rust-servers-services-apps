# rust-servers-services-apps
rust learning

```sh
PS D:\code\rust\rust-servers-services-apps\scenario1> git pull https://gitFrom https://github.com/telegong/rust-servers-services-apps
fatal: refusing to merge unrelated histories
PS D:\code\rust\rust-servers-services-apps\scenario1> git status          hub.com/telegong/rust-servers-services-apps.git master
On branch master
nothing to commit, working tree clean
PS D:\code\rust\rust-servers-services-apps\scenario1> git pull origin master --allow-unrelated-histories
From https://github.com/telegong/rust-servers-services-apps
 * branch            master     -> FETCH_HEAD
Auto-merging .gitignore
CONFLICT (add/add): Merge conflict in .gitignore
Automatic merge failed; fix conflicts and then commit the result.
PS D:\code\rust\rust-servers-services-apps\scenario1> git add .
PS D:\code\rust\rust-servers-services-apps\scenario1> git commit -m "Resolve merge conflicts"
[master 245d7ef] Resolve merge conflicts
PS D:\code\rust\rust-servers-services-apps\scenario1>
```