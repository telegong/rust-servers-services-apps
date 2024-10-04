# rust-servers-services-apps
rust learning

### 1. scenario1 github repo. sync
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

## 2. scenario1 TCP server

```sh
PS D:\code\rust\rust-servers-services-apps\scenario1> dir


    디렉터리: D:\code\rust\rust-servers-services-apps\scenario1

Mode                 LastWriteTime         Length Name                                                                                                   
----                 -------------         ------ ----                                                                                                   
d-----      2024-10-04   오후 6:06                http                                                                                                   
d-----      2024-10-04   오후 6:06                httpserver                                                                                             
d-----      2024-10-04   오후 6:06                src                                                                                                    
d-----      2024-10-04   오후 6:06                tcpclient                                                                                              
d-----      2024-10-04   오후 6:06                tcpserver                                                                                              
-a----      2024-10-04   오후 6:06            898 .gitignore                                                                                             
-a----      2024-10-04   오후 6:06            169 Cargo.toml                                                                                             
-a----      2024-10-04   오후 6:06           1038 readme.md


PS D:\code\rust\rust-servers-services-apps\scenario1> cargo run -p tcpserver
     Locking 5 packages to latest compatible versions
   Compiling tcpserver v0.1.0 (D:\code\rust\rust-servers-services-apps\scenario1\tcpserver)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 1.33s
     Running `target\debug\tcpserver.exe`
Running on port: 3000
Connection established

```

## 3. scenario1 TCP client

```sh
PS D:\code\rust\rust-servers-services-apps\scenario1> cargo run -p tcpclient
   Compiling tcpclient v0.1.0 (D:\code\rust\rust-servers-services-apps\scenario1\tcpclient)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.62s
     Running `target\debug\tcpclient.exe`
Got response from server: "Hello"
PS D:\code\rust\rust-servers-services-apps\scenario1>   
```
