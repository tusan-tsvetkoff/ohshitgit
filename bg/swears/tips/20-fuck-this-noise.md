---
tags: tip
title: Ебал съм го в хаоса, предавам се.
id: fuck-this-noise
note: this should always be the last one in the list, so setting order to 20 so I don't have to re-name/re-order it
order: 20
---

```git
cd ..
sudo rm -r shibana-git-repo-papka
git clone https://some.github.url/shibana-git-repo-papka.git
cd shibana-git-repo-papka
```

Благодаря на Ерик В. за това. Всички оплаквания от употребата на `sudo` в тази шега моля адресирайте към него.

Но наистина, ако бранча ти е толкова наебан, че трябва да върнеш състоянието на репото да е същото като римоут репото по "угоден за гит" начин, пробвай това, но имай предвид, че това са разрушителни и невъзстановими действия!

```git
# вземи последното състояние на ориджин
git fetch origin
git checkout master
git reset --hard origin/master
# изтрий файлове и директории, които не се следят от гит
git clean -d --force
# repeat checkout/reset/clean за всеки наебен бранч
```
