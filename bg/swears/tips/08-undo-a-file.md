---
tags: tip
title: Деба, трябва да върна промените в един файл!
id: undo-a-file
order: 8
---

```git
# намери хаш на комит преди файла да е бил променен
git log
# ползвай стрелките да се движиш нагоре и надолу в историята
# след като си намериш комита, запази хаша
git checkout [saved hash] -- path/to/file
# старата версия на файла ще бъде в индекса ти
git commit -m "Ebasi, ne trqbva da copy paste-vash za da vurnesh promeni!"
```

Когато най-накрая го схванах, беше СИЛНО. СИЛНО. С-И-Л-Н-О. Така де, на кой шибан свят `checkout --` има логика да е най-добрият начин да върнеш файл? :shakes-fist-at-linus-torvalds:
