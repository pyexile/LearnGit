hello world
2. 测试：直接在远程库修改，看本地使用pull之后的结果，是本地能直接被修改，还是要手动修改
   结果：（若只是远程库修改，本地为修改该文件，那么pull之后，本地的文件里会自动修改）
3. 
   git init:初始化本地的一个目录，将它变为可管理的仓库
   git status:查看当前目录中的文件和work space中的差异（即查看是否有文件被修改）
   git add file:
   git commit -m '描述':如果有多个文件被修改，最好每个文件都执行以下git add file，而不要git add .，因为执行git add file之后，可以紧跟着执行commit，这样提交之后，你的每个文件都对应了不同的描述，便于别人和自己查看
   git diff file:当有文件被修改时，想要查看这个文件修改了什么，可以使用git diff file查看
4. 版本回退
   版本类似于快照，每次执行git commit命令，其实就是增加一个版本
   git log:查看所有版本，如果想要显示的内容比较清晰，可以使用git log --pretty=oneline
   git reset --hard HEAD^:回退到上一个版本，也就是上一次提交commit时文件的样子
   git reflog:显示你之前是哟用过的命令，这样如果你版本回退后，又想回到回退前，那么使用该命令查看之前使用过的命令，然后找到上一回执行回退命令那个地方，找到执行回退时上一回的版本号的id，然后执行git reset --hard id号，就可以了。
   HEAD表示当前版本，HEAD^表示上一个版本，类推HEAD^^，回退的多时，例如回退100，那么就是用HEAD~100

5. 工作区和暂存区
   .git是Git的版本库，Git的版本库里存了很多东西，其中最重要的就是称为stage（或者叫index）的暂存区，还有Git为我们自动创建的第一个分支master，以及指向master的一个指针叫HEAD。
   工作区就是我们的工作目录，当执行git add file之后，其实就是将文件file传到暂存区，然后使用git commit 时，就是将暂存区的内容全部提交到当前分支
