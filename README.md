## Laboratory work XII

Данная лабораторная работа посвещена изучению специализированного текстового редактора **Vim**

```bash
$ open https://ru.wikipedia.org/wiki/Vim
```

## Tasks

- [ ] 1. Создать публичный репозиторий с названием **lab12** на сервисе **GitHub**
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Ознакомиться со ссылками учебного материала

## Tutorial

```bash
$ export GITHUB_USERNAME=<имя_пользователя>
```

```bash
$ vimtutor ru
```

```bash
$ git clone https://github.com/${GITHUB_USERNAME}/lab11 lab12
$ cd lab12
$ git remote remove origin
$ git remote add origin https://github.com/${GITHUB_USERNAME}/lab12
```

```bash
$ vim README.md
:s/lab11/lab12/g
/file<CR>wChaving the path environment variable value **LOG_PATH**
:wq
```

```bash
$ vim sources/demo.cpp
Yp3wct>cstdlib<ESC>
8Gostd::string log_path = std::getenv("LOG_PATH");
/"log<CR>
cf"log_path<CR>
k2dd2kpVj<<
:wq
```

```bash
$ cd $HUNTER_ROOT
$ git create
$ git release create v0.18.57.1
$ git release show v0.18.57.1
```

```bash
$ wget https://github.com/${GITHUB_USERNAME}/hunter/archive/v0.18.57.1.tar.gz
$ export MYHUNTER_SHA1=`openssl sha1 v0.18.57.1.tar.gz | cut -d'=' -f2 | cut -c2-41`
$ echo $MYHUNTER_SHA1
```

```
$ echo $MYHUNTER_SHA1 | pbcopy
$ vim CMakeLists.txt
/SHA1<CR>
wcw<C-V><CR>
:wq
```

```bash
$ git add .
$ git commit -m"refactoring"
$ git push origin master
```

## Links

- [ex](https://en.wikipedia.org/wiki/Ex_(text_editor))
- [vi](https://en.wikipedia.org/wiki/Vi)