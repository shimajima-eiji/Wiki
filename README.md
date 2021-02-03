# このリポジトリはWikiでありサイトでありコメントフォームとして扱う
Gitコマンドを使わず、ブラウザだけを使ってGithubを運用する事を考えるリポジトリ<br />
すべてのリポジトリのmainブランチ（リポジトリ）という位置付けにする。<br />
[Issues](https://github.com/shimajima-eiji/Wiki/issues)はリポジトリを横断的に扱う事ができる。

# 管理方法
すべてのリポジトリで、本来リポジトリとして独立させるべき機能を成立させる。<br />
Slackチャンネルのように、親子関係にあるものは命名規則に準拠する<br />
ただし、Githubで特殊な意味を持つリポジトリ
- [[アカウント名]](https://github.com/shimajima-eiji/shimajima-eiji)
- [[アカウント].github.io](https://github.com/shimajima-eiji/shimajima-eiji.github.io)

と

- [Gist](https://github.com/shimajima-eiji/Gist)

は本リポジトリ直下で管理する。

## 注意
- [[アカウント名].github.io](https://github.com/shimajima-eiji/shimajima-eiji.github.io)はHostingの親ではない
- ややこしいので、GithubPagesを使う場合はリポジトリ名の最後に[_GHP]を付与する

# リポジトリツリー
## 特殊なもの
Githubの仕様に基くもの

- Wiki: 運用管理
  - [[アカウント名]](https://github.com/shimajima-eiji/shimajima-eiji): README.mdにはGithubプロフィールで公開したいものを、その他はREADME.mdからリンクを貼るコンテンツなど
  - [[アカウント].github.io](https://github.com/shimajima-eiji/shimajima-eiji.github.io): GithubPagesでルートとなるもの。運用は未定だがGoogleなどサービスの審査対象となる。
  - [Gist](https://github.com/shimajima-eiji/Gist): Gistをサブモジュールに集約するもの

## 親リポジトリ
外部サイトとは、GithubPagesを含む。

- JAMStack_: 外部サイトで公開しているもので、特にブログやサイトなど公開したいコンテンツを持っている場合はHostingではなくこちらに該当する
- Hosting_: 外部サイトで公開しているもの。基本的にprivateで運用される事を想定
- [GAS_](https://script.google.com/home): GASプロジェクトで使用しているもの。基本的にprivateで運用される事を想定
- [RevealJS_](https://revealjs.com): 外部サイトで公開しているもので、特にプレゼンテーションやLTなど公開したいコンテンツを持っている場合は、Hostingではなくこちらに該当する

単独で完結するリポジトリについては上記制限の対象外。
