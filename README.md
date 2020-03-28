# Centos-Git-Guide
将本地代码、文件提交到GitHub 步骤：

第一步：cd 到你的本地项目根目录下，执行git命令  目的是建立git仓库  
git init

第二步：将项目的所有文件添加到仓库中  
git add .

第三步：将add的文件commit到仓库  
git commit . -m "备注文字"  

第四步：去github上创建自己的Repository，创建后的页面如下图所示：  

点击Clone or download按钮，复制弹出的地址git@github.com:***/test.git，记得要用SSH的地址，尽量不要用HTTPS的地址，如上图所示

第五步：将本地的仓库关联到github上---把上一步复制的地址放到下面  
git remote add origin git@github.com:***/test.git

第六步：上传github之前，要先pull一下，执行如下命令：  
git pull origin master   (有时会提示失败 fatal: Couldn't find remote ref master 但不用管,继续执行下一条命令)

第七步，上传代码到github远程仓库  
git push -u origin master
