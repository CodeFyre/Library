# دليل Git و GitHub الكامل للمبتدئين حتى الاحتراف

هذا الدليل يحتوي على أكثر من 50 أمر Git مع شرح بسيط لكل أمر.
الملف مكتوب بصيغة Markdown وجاهز للاستخدام داخل Visual Studio Code.

## 1. التحقق من تثبيت Git

```bash
git --version
```

يعرض إصدار Git المثبت على الجهاز.

## 2. إعداد Git لأول مرة

### تعيين اسم المستخدم

```bash
git config --global user.name "Your Name"
```

### تعيين البريد الإلكتروني

```bash
git config --global user.email "you@example.com"
```

### عرض إعدادات Git

```bash
git config --list
```

## 3. إنشاء مستودع جديد

```bash
git init
```

يقوم بإنشاء مستودع Git جديد داخل المشروع.

## 4. استنساخ مستودع من GitHub

```bash
git clone https://github.com/username/repository.git
```

ينسخ مشروع موجود من GitHub إلى جهازك.

## 5. التحقق من حالة المشروع

```bash
git status
```

يعرض الملفات المعدلة أو غير المتعقبة.

## 6. إضافة ملف واحد إلى منطقة التتبع

```bash
git add file.txt
```

## 7. إضافة جميع الملفات

```bash
git add .
```

## 8. إضافة عدة ملفات

```bash
git add file1.js file2.js
```

## 9. إنشاء Commit

```bash
git commit -m "Initial commit"
```

يقوم بحفظ التعديلات في تاريخ المشروع.

## 10. عرض سجل التعديلات

```bash
git log
```

## 11. عرض سجل مختصر

```bash
git log --oneline
```

## 12. عرض التعديلات بين الملفات

```bash
git diff
```

## 13. عرض التعديلات لملف معين

```bash
git diff file.txt
```

## 14. ربط المشروع بمستودع GitHub

```bash
git remote add origin https://github.com/username/repository.git
```

## 15. عرض المستودعات البعيدة

```bash
git remote -v
```

## 16. رفع المشروع إلى GitHub

```bash
git push -u origin main
```

## 17. سحب التحديثات من GitHub

```bash
git pull origin main
```

## 18. تحميل التحديثات فقط

```bash
git fetch
```

## 19. إنشاء فرع جديد

```bash
git branch new-feature
```

## 20. عرض الفروع

```bash
git branch
```

## 21. الانتقال إلى فرع

```bash
git checkout new-feature
```

## 22. إنشاء فرع والانتقال له مباشرة

```bash
git checkout -b new-feature
```

## 23. حذف فرع

```bash
git branch -d branch-name
```

## 24. دمج فرع مع الفرع الحالي

```bash
git merge branch-name
```

## 25. إعادة تسمية فرع

```bash
git branch -m new-name
```

## 26. حذف فرع من GitHub

```bash
git push origin --delete branch-name
```

## 27. إلغاء تعديل ملف

```bash
git checkout -- file.txt
```

## 28. إزالة ملف من staging

```bash
git reset file.txt
```

## 29. تعديل آخر commit

```bash
git commit --amend
```

## 30. حفظ العمل مؤقتاً

```bash
git stash
```

## 31. استعادة العمل المؤقت

```bash
git stash pop
```

## 32. عرض قائمة stash

```bash
git stash list
```

## 33. حذف stash

```bash
git stash drop
```

## 34. إنشاء Tag

```bash
git tag v1.0
```

## 35. عرض جميع Tags

```bash
git tag
```

## 36. رفع Tag إلى GitHub

```bash
git push origin v1.0
```

## 37. عرض تفاصيل Commit

```bash
git show commitID
```

## 38. البحث في سجل التعديلات

```bash
git log --grep="bug fix"
```

## 39. معرفة من عدل الكود

```bash
git blame file.js
```

## 40. استعادة Commit

```bash
git revert commitID
```

## 41. إعادة المشروع إلى Commit سابق

```bash
git reset --hard commitID
```

## 42. إعادة المشروع بدون حذف التعديلات

```bash
git reset --soft HEAD~1
```

## 43. عرض الملفات المتعقبة

```bash
git ls-files
```

## 44. حذف ملف من Git

```bash
git rm file.txt
```

## 45. حذف ملف من Git فقط دون حذفه من الجهاز

```bash
git rm --cached file.txt
```

## 46. نقل أو إعادة تسمية ملف

```bash
git mv old.txt new.txt
```

## 47. إنشاء commit فارغ

```bash
git commit --allow-empty -m "empty commit"
```

## 48. عرض آخر commit

```bash
git log -1
```

## 49. معرفة الفرع الحالي

```bash
git branch --show-current
```

## 50. تحديث جميع الفروع

```bash
git fetch --all
```

## 51. تنفيذ rebase

```bash
git rebase main
```

## 52. إلغاء rebase

```bash
git rebase --abort
```

## 53. إلغاء merge

```bash
git merge --abort
```

## 54. رفع فرع جديد إلى GitHub

```bash
git push origin branch-name
```

## 55. رفع جميع الفروع

```bash
git push --all
```

## 56. رفع جميع الـ Tags

```bash
git push --tags
```

## 57. استنساخ مستودع مع فرع محدد

```bash
git clone -b branch-name repo-url
```

## 58. عرض حجم المستودع

```bash
git count-objects -vH
```

## 59. تنظيف الملفات غير المتعقبة

```bash
git clean -f
```

## 60. ضغط المستودع

```bash
git gc
```

## 61. فحص سلامة المستودع

```bash
git fsck
```

## نصائح مهمة

* استخدم git status قبل كل commit
* استخدم الفروع لتجربة الميزات الجديدة
* لا ترفع الملفات الحساسة إلى GitHub
* استخدم ملف .gitignore لتجاهل الملفات غير المهمة

هذا الدليل يغطي أهم أوامر Git التي يحتاجها المطور من المستوى المبتدئ حتى المستوى المتقدم.
