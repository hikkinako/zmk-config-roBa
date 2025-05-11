# build方法  
1. docker desktopを立ち上げる


2. 下記実行
```powershell
powershell -ExecutionPolicy Bypass -File .\scripts\build.ps1
```


# keymap
![image](https://github.com/user-attachments/assets/932f2ca1-e3c8-43d4-b4d3-c1e14d3bc406)
![image](https://github.com/user-attachments/assets/21a826d4-375f-4f11-8cd6-a74413a3f8d9)
![image](https://github.com/user-attachments/assets/28feb1f5-71d4-428d-926d-1bd6c9b35442)
![image](https://github.com/user-attachments/assets/0f90bd5d-4100-4e57-aa67-5852a3099469)
![image](https://github.com/user-attachments/assets/6c61b480-338f-4b78-86c6-c5a37112b34b)
![image](https://github.com/user-attachments/assets/bfda4a6d-9c70-45a0-aa1d-ff0b076dd64e)





# docker設定
https://github.com/kot149/zmk-config-roBa/blob/main/docs/build_locally.md

```docker
docker volume create --driver local -o o=bind -o type=none -o device="C:\Users\hinak\Documents\Program\keyboard\roba\zmk-config-roBa\" zmk-config
```
```docker
docker volume create --driver local -o o=bind -o type=none -o device="C:\Users\hinak\Documents\Program\keyboard\roba\zmk-modules\" zmk-modules
```

ZMKのコンテナ作成
クローンしたzmkディレクトリをVSCodeで開く。

Command PaletteからRemote: Show Remote Menuを実行し、Reopen in Containerを選択する。

コンテナが作成され、コンテナ内の/workspaces/zmk/ディレクトリでVSCodeが開かれる。