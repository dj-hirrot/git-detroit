# git-detroit
**git-detroit** をインストールすると, 不要なローカルブランチを一括で削除できます.   
インストールには [HomeBrew](https://brew.sh/) を使用するので, 先にインストールしておいてください.

# Installation

```bash
$ brew tap dj-hirrot/git-detroit
$ brew install git-detroit
```

# Usage
💥 **git-detroit で削除の対象になるのは, 接頭辞に `features/` がつくブランチのみです.** 💥

**git-detroit** はGit管理下にあるプロジェクトでのみ動作します.
なので, まずはブランチを整理したいディレクトリまで移動します.

```bash
$ cd ~/path/to/repogitory
```

たったこれだけで **git-detroit** が使用できるようになります.   

```bash
$ git-detroit
=> do you remove feature/xxxxx_xxxxx ? (y/n): y
Deleted branch feature/xxxxx_xxxxx (was xxxxxx).
```

# Idea
**git-detroit** をインストールしたら, まずはエイリアスを作成することをお勧めします.

```bash
$ echo "alias gdes='git-detroit'" >> ~/.alias
```

