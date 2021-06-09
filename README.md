> 本组织下的所有仓库，均采用MIT开源协议，全部免费商用
# 微服务框架：酸菜
一个功能、页面，或者一个按钮，都可以是一个服务

# 分支说明
- feature：用于开发的分支，自测完成后，合并 develop分支，然后提交到该 feature分支（不提交到 develop分支），再然后提交到 release分支进行测试，该 feature分支可删除，也可不删除，不删除的话就不允许改变了
- develop：相对稳定的开发环境分支，就是测试通过后的分支，会合并到 develop分支，然后 master分支来合并 develop分支
- master：生产环境分支
- release：该分支用于测试人员进行测试，测试不通过，则在这个 release分支上进行修改，测试通过之后，develop分支来合并这个 release分支，该 release分支可删除，也可不删除，不删除的话就不允许改变了
- hotfix：master分支上线后出现问题，从 master分支拉取代码，然后修改，然后提交（此时不合并 develop了），然后 master和 develop分支，去合并这个 hotfix分支，该 hotfix分支可删除，也可不删除，不删除的话就不允许改变了，如果问题未修复，则从 master拉取新的 hotfix继续修改
- 说白了就是：feature开发，然后就变成了release测试分支，如果测试有问题，则在release上修改提交，测试完成之后 develop整合 release分支，master把 develop分支上线，上线之后有问题，就在 hotfix分支上修改并测试，然后 master和 develop分支，去合并 hotfix分支

# 项目历程

- 2021-04-26：项目成立，定一个小目标：进入 中国开源项目 应用软件类排行榜 [2020排行榜地址](https://www.oschina.net/project/top_cn_2020?sort=1)
