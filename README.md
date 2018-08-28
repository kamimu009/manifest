# manifest

1. set ssh config

    ```shell
    $ nano ~/.ssh/config
    
    Host review.gerrithub.io
    HostName     review.gerrithub.io
    Port         29418
    User         XXXX
    ```
1. install repo

    ```shell
    curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
    chmod a+x ~/bin/repo
    ```
    > https://source.android.com/setup/build/downloading  
1. create dhirectory

    ```shell
    $ mkdir rise-app
    $ cd rise-app
    ```
1. repo init

    ```shell
    $ repo init -u ssh://review.gerrithub.io:29418/kamimu009/manifest
    ```
1. repo sync

    ```shell
    $ repo sync
    ```

Done!
