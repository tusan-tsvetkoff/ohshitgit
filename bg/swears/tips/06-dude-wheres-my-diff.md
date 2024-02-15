---
tags: tip
title: Деба, пробвах се да рънна "диф", но нищо не стана?!
id: dude-wheres-my-diff
order: 6
---

If you know that you made changes to files, but `diff` is empty, you probably `add`-ed your files to staging and you need to use a special flag.
Ако знаеш, че си направил промени във файлове, но `diff` е празен, най-вероятно си `add`-нал файловете в стейджинг и трябва да ползваш специален флаг.

```git
git diff --staged
```

Файл под &macr;\\\_(ツ)\_/&macr; (да, знам, че така си функционира, не е бъг, но мамка му, много е объркващо и изобщо не е очевидно, когато ти се случи за пръв път!)
