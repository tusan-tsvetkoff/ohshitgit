---
tags: tip
title: Деба, без да искам комитнах в грешния бранч!
id: accidental-commit-wrong-branch
order: 5
---

```git
# върни последния комит, но остави промените
git reset HEAD~ --soft
git stash
# move to the correct branch
# иди в правилния бранч
git checkout imeto-na-pravilniq-branch
git stash pop
git add . # or добави индивидуални файлове
git commit -m "suobshtenieto ti";
# now your changes are on the correct branch
# сега промените ти са на правилния бранч
```

Много хора предлагат ползването на `cherry-pick` в тази ситуация, така че избери това, което ти се струва за правилно!

```git
git checkout imeto-na-pravilniq-branch
# вземи последния комит от мастър
git cherry-pick master
# изтрий го от мастър
git checkout master
git reset HEAD~ --hard
```
