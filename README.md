# macbook-provisioning

## 参考
- [Mac の開発環境構築を自動化する (2015 年初旬編)](http://t-wada.hatenablog.jp/entry/mac-provisioning-by-ansible)

## 実行コマンド
- `HOMEBREW_CASK_OPTS="--appdir=/Applications" ansible-playbook -i hosts -vv localhost.yml`

## brew caskのインストール方法変更あり。対応ログ
- homebrew_cask_packagesのタスクが失敗するようになった。
- [ここ](http://rcmdnk.github.io/blog/2015/12/18/computer-homebrew-brew-file-mac/)を参考に、`brew uninstall --force brew-cask; brew update` することで解決。
