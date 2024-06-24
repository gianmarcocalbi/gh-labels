# gh-labels

A repository to manage GitHub labels.

## Naming convention

Labels are named like `<category> • <name>` where `<category>` is one of the
following:

- `c` for _component_: the part of the software that is concerned by the issue.
- `k` for _kind_: the kind of the issue (e.g., bug, feature).
- `m` for _miscellaneous_: labels that do not fit in any other category.
- `o` for _origin_: the origin of the issue (e.g., feedback, dev).
- `p` for _product_: the product that is concerned by the issue. If the
  repository contains a single product, this category is not used.
- `r` for _resolution_: the resolution of the issue (e.g., invalid, duplicate).
- `t` for _topic_: the topic of the issue (e.g., security, performance).

__Always assign a label of the `k` category__. Usually one, but sometimes an
issue can have multiple labels of `k` category, e.g., an issue is opened as
something is not working > `k • bug`, but the bug requires a fix to be
implemented > assign also `k • fix` label.

## Usage

To set labels for a repository, run the following command:

```bash
wget -O - https://raw.githubusercontent.com/gianmarcocalbi/gh-labels/main/scripts/gh-labels | bash
```

__Note__: running this script will delete all labels currently in the repository.
