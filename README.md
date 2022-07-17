# Linux-CrossCompile-Env
Visual Studio Codeでクロス開発を行うためのDockerコンテナと設定ファイル一式\
Ubuntu上で扱うことを前提に設計しているため、その他のOSは適時読み替えが必要。\
ビルドタスクはクロスコンパイル->rsyncで同期の流れで行う。\
デバッグは上記に加え、sshコマンドでリモート上のマシンでgdbserverを起動させ、ホスト側と接続して行う。\
そのため、リモート側には予めgdbserverのインストールが必要。\
リモートマシンのIPアドレス/ホスト名とユーザ名は.devcontainer/devcontainer.jsonで編集。\
公開鍵認証でsshできるようにすることを推奨。
