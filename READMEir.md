دستورات گیت
============

## نسخه های ترجمه شده
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [persian version](READMEir.md)
- [العربية](READMEar.md)

___

_فهرستی از دستورات گیت که معمولاً استفاده می کنم_

*اگر به نام مستعار گیت من علاقه دارید، به `bash_profile.` من که در اینجا یافت می شود نگاه کنید: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### دریافت و ایجاد پروژه ها

| دستور | توضیحات |
| ------- | ----------- |
| `git init` | ایجاد یک ریپوزیتوری یا مخزن در لوکال |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | کپی کردن یک ریموت ریپوزیتوری در لوکال |

### مبانی

| دستور | توضیحات |
| ------- | ----------- |
| `git status` | بررسی کردن وضعیت |
| `git add [file-name.txt]` | اضافه کردن یک فایل به استیجینگ |
| `git add -A` | اضاغه کردن همه ی فایل های جدیدِ تغییر یافته به استیجینگ |
| `git commit -m "[commit message]"` | ثبت تغییرات با پیام مناسب |
| `git rm -r [file-name.txt]` | حذف کردن یک فایل یا فولدر |
| `git remote -v` | دیدن ریموت ریپوزیتوری از فایل یا دایرکتوری فعلیِ در حال کار |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |
| `git stash pop` | Apply latest stash to working directory |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
