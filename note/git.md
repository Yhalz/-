*增删改查*
**ls**
ls -a //查看以.开头的文件
**查**
pwd                 // 查看当前目录绝对路径
ls                  // 查看当前目录内容
cat 路径            // 查看文件内容
head 路径           // 前十(-n 指定)行
tail 路径           // 后十(-n 指定)行
less 路径           // 选择查看 q退出 选中状态esc后q退出
**增**
touch 文件名        // 增加文件
echo 111 > 文件名   // '>'覆盖111到文件名中 '>>'追加111到文件名中 -e "111\n222"追加可换行输入(\n)
mkdir 文件夹        // 创建文件夹 -p 创建层级目录
copy -r 文件复制    // 复制文件夹及其内容
**删**
rm 文件             // 删除文件
echo $?             // 查看命令执行结果 errorcode为0为成功 为1或者其他code为失败
rm 文件名 && echo 删除成功 // 删除并返回删除结果

***组合使用***
rm 文件名 && touch 文件名 && rm 文件名 && echo 成功 // 从前到后执行 卡住则失败
rm 文件名; echo 执行完毕                           // 从前到后执行 无论结果如何都继续执行
{脚本文件}
start/code 打开文件
./文件名
sh 文件名           // 可一键执行增删改查命令(脚本)
***shebang***
#!/usr/bin/env 语言 //删掉语言也能执行
                    //加了PASH才可以只用文件名执行
**git**
git init //创建.git目录
git add 目录or文件名 //添加到git仓库 删除文件提交 
.gitignore //标记不需要提交的文件名 就不会显示了
git status //查看
git commit -m 版本号 or 字符串（更新内容） //commit
git commit -v//使用vasode提交
git log //查看拷贝几次拷贝了什么
git reset --hard xxxxx//版本切换
git reflog //查看所有操作 包括版本回退
start .//打开当前文件
git branch x //创造x分支
git branch //不用跟参数 可查看当前有多少分支
git checkout x//切换到x分支 git stash 合并冲突
git merge x//将x分支与master分支合并 冲突就code 打开文件修改
git status -sb //查看出错的文件
git branch -d x//删除x分支

git remote add origin git@github.com:Yhalz/-.git
git branch -M main
git push -u origin main