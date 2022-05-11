# Github_HW_2

1. На Локальном репозитории сделать ветки для:

- Postman  
`git branch Postman`

- Jmeter  
`git branch Jmeter`

- CheckLists  
`git branch CheckLists`

- Bug Reports  
`git branch Bug_Reports`

- SQL  
`git branch SQL`

- Charles  
`git branch Charles`

- Mobile testing  
`git branch Mobile_Testing`

2. Запушить все ветки на Внешний репозиторий  

`git push -u origin --all`

3. В ветке **Bug Reports** сделать текстовый документ со структурой баг репорта  

`git checkout Bug_Reports`  
`touch bug_report.txt`  
`vim bug_report.txt`  
<pre><kbd>i</kbd></pre>  
```
1. ID
2. Project
3. Summary
4. Actual result
5. Expected result
6. Pre-conditions
7. Steps to reproduce
8. Environment
9. Severity
10. Priority
11. Status
12. Attachments
13. Reporter
14. Workaround
15. Reproducibility
```
<pre><kbd>esc</kbd></pre>  
`:wq`  

4. Запушить структуру багрепорта на Внешний репозиторий  

`git add . ; git commit -m "add bug_report.txt" ; git push`

5. Вмержить ветку **Bug Reports** в **main**  

`git checkout main`  
`git merge Bug_Reports`  

6. Запушить **main** на Внешний репозиторий  

`git push`  

7. В ветке **CheckLists** набросать структуру чек листа  

`git checkout CheckLists`  
`touch checklist.txt`  
`vim checklist.txt`  
<pre><kbd>i</kbd></pre>  
```
1. Built
2. Environment
3. Tester
4. Module
5. ID
6. Test Type
7. Checking
8. Result
9. Defect
```
<pre><kbd>esc</kbd></pre>  
`:wq`  

8. Запушить структуру на Внешний репозиторий  

`git add . ; git commit -m "add checklist.txt" ; git push`  

9. На Внешнем репозитории сделать *Pull Request* ветки **CheckLists** в **main**  

Перейти на [github.com](https://github.com) в нужный репозиторий >> `Compare & pull request` >> `Create pull request` >> `Merge pull request` >> `Confirm merge`  

10. Синхронизировать Внешнюю и Локальную ветки **main**  

`git checkout main`  
`git pull`  
