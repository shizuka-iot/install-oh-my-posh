# install-oh-my-posh
oh-my-poshの導入方法メモ
[参考](https://docs.microsoft.com/ja-jp/windows/terminal/tutorials/powerline-setup)

## 開発環境
windows10 home
windows powershell

## 事前に必要なもの
* windows terminal
* 文字化けしないフォント

## やりかた
1. powershellで下記コマンド

  Install-Module posh-git -Scope CurrentUser
  Install-Module oh-my-posh -Scope CurrentUser
  
2. powershellで`notepad $PROFILE`で設定ファイルを開き（なければ作る）下記を追記

  Import-Module posh-git
  Import-Module oh-my-posh
  Set-PoshPrompt -Theme gmay
