hello world
2. 测试：直接在远程库修改，看本地使用pull之后的结果，是本地能直接被修改，还是要手动修改
   结果：（若只是远程库修改，本地为修改该文件，那么pull之后，本地的文件里会自动修改）
3. 
   git init:初始化本地的一个目录，将它变为可管理的仓库
   git status:查看当前目录中的文件和work space中的差异（即查看是否有文件被修改）
   git add file:
   git commit -m '描述':如果有多个文件被修改，最好每个文件都执行以下git add file，而不要git add .，因为执行git add file之后，可以紧跟着执行commit，这样提交之后，你的每个文件都对应了不同的描述，便于别人和自己查看
   git diff file:当有文件被修改时，想要查看这个文件修改了什么，可以使用git diff file查看
   
