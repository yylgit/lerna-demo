第一种方法
这个是3.10的高版本
lerna publish --skip-git  先发布子包  此时代码的version 都没有变
lerna version --no-git-tag-version --no-push  再改变版本
也可以给cli安装子包  
测试没有问题 
统一提交版本修改并打tag

第二种方法
lerna publish --no-git-tag-version --no-push  子包发布成功   没有提交 版本号也改了  显示lerna命令失败



可能lerna版本的问题

npm run 中的就不会自动改变版本 这个是高版本3.10


直接执行的就可以

lerna publish --no-git-tag-version --no-push  

