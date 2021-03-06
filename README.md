# Github Labels

Add github labels automatically.

It's very useful that init all your custom labels when create a repo.

---

## Install

```
$ npm install github-labels -g
```

## Usage

```
$ labels -c path/to/conf.json user/repo
```

About config file, see [my conf](https://github.com/popomore/dotfile/blob/master/conf/labels.json) for example.

```
[
  {"name": "bug", "color": "ffffff"},
  {"name": "feature", "color": "000000"}
]
```

Your can simplify it that will generate github default color automatically.

```
["bug", "feature"]
```

Force option will delete all existing labels, otherwise will create label when not exist or update label when existing label has different color.

```
$ labels -c path/to/conf.json -f user/repo
```

## Lisence

MIT
