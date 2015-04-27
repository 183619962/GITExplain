####git基础操作说明
1.**初始化本地git仓库**

 - git  init
 >cd 文件夹路径（进入指定的文件 如：cd /d/mywork）

 >mkdir 文件夹名称（创建一个文件夹 如：mkdir demoWork）

 >pwd 显示当前所在的位置的路径


2.**添加文件到git仓库**

 - git add 文件名 如：git add file.txt
 >如果想偷懒可以使用如下指令：git add .（表示添加所有的文件）

 - git commit -m "提交描述" 如：git commit -m “first commit”


>以上为初始化的操作和提交，提交之后进行下一步的开发


3.查看文件的状态，如果修改会有相应的展示

- git status


4.查看详细修改的地方

- git diff 文件名 如：git diff file.txt

5.查看文件的内容

- cat 文件名(如：cat file.txt)


6.提交修改后的代码，执行第二条说明中的相关指令


7.查看提交记录

- git log或git log --pretty=oneline
 >会由近到远展示所有的提交记录

 >git log --pretty=oneline展示的信息更加简洁易读。如下：

 >3628164fb26d48395383f8f31179f24e0882e1e0 第三次提交

 >ea34578d5496d7dd233c827ed32a8cd576c5ee85 第二次提交

 >cb926e7ea50ad11b8f9e909c05226233bf755030 第一次提交


8.撤销到上一步的提交

 - git reset --hard HEAD^
 >可以通过git log查看提交日志

 >可以通过cat file.txt来查看当前文件的版本信息



9.通过上面的操作退回到了上一步，如何再退回来

- git reset --hard 3628164
>后面跟的是commit id的前几位，不需要写全，也不能太短，能唯一标识提交的ID


