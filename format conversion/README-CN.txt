# 格式转换[¶](http://www.worldhello.net/gotgithub/#gotgithub "永久链接至标题")

<colgroup><col> <col></colgroup>
| Author: | Jiang Xin |
| Version: | v0.9.1-13-g5075479 |
| Copyright: | [Creative Commons BY-NC-SA](http://creativecommons.org/licenses/by-nc-sa/3.0/) |

<div>

## 前言[¶](http://www.worldhello.net/gotgithub/#id1 "永久链接至标题")

动笔写GitHub不是因为我对其了解，恰恰是对其太不了解。

在我的《Git权威指南》 [[1]](http://www.worldhello.net/gotgithub/#id4) 一书中，涉及到GitHub的只有区区三页纸，这显然回答不了读者对于GitHub的诸多疑问。 记得在《Git权威指南》刚刚完稿之际，机械工业出版社华章公司的杨福川编辑就鼓动我写一本关于GitHub的书，我用了好多理由推辞了。 头条理由就是我真的累着了。在每一章节开始动笔之时，都好像是坐在了中学语文考试的考堂上写作文，时间快到了可仍然动不了笔， 再写一本书无疑要重复这一痛苦的经历。 第二个理由是我更喜欢编程，而不是写文档，尤其写GitHub会有大量截图、图像处理的琐碎工作。 第三个理由彻底让编辑投降，那就是GitHub是一个国外网站，也许书一出，【此句已被原作者删除】。

让我最终决定动笔，是源于CSDN蒋总在美国拜访GitHub总部后告诉我的一些见闻，我对GitHub如此成功运作产生了兴趣，于是开始研究GitHub的博客，愈发发现GitHub是一群有趣的人在做的有趣的事，如果只把GitHub当作一个Git服务器，实在是暴殄天物。GitHub已经并将继续获得成功，若真能凭借此书把GitHub尽量全面地展现，让每一个Git使用者用好GitHub也是一件幸事。

这本书将采用GitHub的方式进行撰写和发布 [[2]](http://www.worldhello.net/gotgithub/#id5) ，任何人都可以看到本书（包括源码），更可以用GitHub的方法参与本书的撰写和纠错。网络出版对于我和杨福川编辑都是一个全新的体验。感谢Git，让我在一年内拥有了两种不同的出版
体验。
> 
– 蒋鑫, 2011.12

* * *

<colgroup><col><col></colgroup>
| [[1]]) | [PDF转MD](http://pdf2md.morethan.io/) |

<colgroup><col><col></colgroup>
| [[2]]) | [html转MD](https://tool.lu/markdown) |
</div>



## 目录[¶](http://www.worldhello.net/gotgithub/#id6 "永久链接至标题")



*   [1\. 探索GitHub](http://www.worldhello.net/gotgithub/01-explore-github/index.html)
    *   [1.1\. 什么是GitHub](http://www.worldhello.net/gotgithub/01-explore-github/010-what-is-github.html)
    *   [1.2\. GitHub亮点](http://www.worldhello.net/gotgithub/01-explore-github/020-github-hightlights.html)
    *   [1.3\. 探索GitHub](http://www.worldhello.net/gotgithub/01-explore-github/030-explore-github.html)
*   [2\. 加入GitHub](http://www.worldhello.net/gotgithub/02-join-github/index.html)
    *   [2.1\. 创建GitHub账号](http://www.worldhello.net/gotgithub/02-join-github/010-account-setup.html)
    *   [2.2\. 浏览托管项目](http://www.worldhello.net/gotgithub/02-join-github/020-browse-repo.html)
    *   [2.3\. 社交网络](http://www.worldhello.net/gotgithub/02-join-github/030-be-social.html)
*   [3\. 项目托管](http://www.worldhello.net/gotgithub/03-project-hosting/index.html)
    *   [3.1\. 创建新项目](http://www.worldhello.net/gotgithub/03-project-hosting/010-new-project.html)
        *   [3.1.1\. 新版本库即是新项目](http://www.worldhello.net/gotgithub/03-project-hosting/010-new-project.html#new-repo)
        *   [3.1.2\. 版本库初始化](http://www.worldhello.net/gotgithub/03-project-hosting/010-new-project.html#init-by-clone)
        *   [3.1.3\. 从已有版本库创建](http://www.worldhello.net/gotgithub/03-project-hosting/010-new-project.html#init-by-push)
    *   [3.2\. 操作版本库](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html)
        *   [3.2.1\. 强制推送](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html#noff-push)
        *   [3.2.2\. 新建分支](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html#new-branch)
        *   [3.2.3\. 设置默认分支](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html#default-branch)
        *   [3.2.4\. 删除分支](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html#del-branch)
        *   [3.2.5\. 里程碑管理](http://www.worldhello.net/gotgithub/03-project-hosting/020-repo-operation.html#git-tags)
    *   [3.3\. 公钥认证管理](http://www.worldhello.net/gotgithub/03-project-hosting/030-repo-authz.html)
        *   [3.3.1\. 用户级公钥管理](http://www.worldhello.net/gotgithub/03-project-hosting/030-repo-authz.html#pubkeys)
        *   [3.3.2\. 项目级公钥管理](http://www.worldhello.net/gotgithub/03-project-hosting/030-repo-authz.html#deploy-keys)
    *   [3.4\. 版本库钩子扩展](http://www.worldhello.net/gotgithub/03-project-hosting/040-repo-hooks.html)
        *   [3.4.1\. 邮件通知功能](http://www.worldhello.net/gotgithub/03-project-hosting/040-repo-hooks.html#mail-notify-hook)
        *   [3.4.2\. 和Redmine整合](http://www.worldhello.net/gotgithub/03-project-hosting/040-repo-hooks.html#redmine)
    *   [3.5\. 建立主页](http://www.worldhello.net/gotgithub/03-project-hosting/050-homepage.html)
        *   [3.5.1\. 创建个人主页](http://www.worldhello.net/gotgithub/03-project-hosting/050-homepage.html#user-homepage)
        *   [3.5.2\. 创建项目主页](http://www.worldhello.net/gotgithub/03-project-hosting/050-homepage.html#project-homepage)
        *   [3.5.3\. 使用专有域名](http://www.worldhello.net/gotgithub/03-project-hosting/050-homepage.html#dedicate-domain)
        *   [3.5.4\. 使用Jekyll维护网站](http://www.worldhello.net/gotgithub/03-project-hosting/050-homepage.html#jekyll)
*   [4\. 工作协同](http://www.worldhello.net/gotgithub/04-work-with-others/index.html)
    *   [4.1\. Fork + Pull模式](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html)
        *   [4.1.1\. 版本库派生](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html#fork)
        *   [4.1.2\. Pull Request](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html#pull-request)
        *   [4.1.3\. 手工合并](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html#merge-by-hands)
        *   [4.1.4\. 在线编辑](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html#online-edit)
        *   [4.1.5\. 简化的 Fork + Pull Request](http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html#fork-pull-request)
    *   [4.2\. 共享版本库](http://www.worldhello.net/gotgithub/04-work-with-others/020-shared-repo.html)
        *   [4.2.1\. 版本库授权](http://www.worldhello.net/gotgithub/04-work-with-others/020-shared-repo.html#collaborators)
        *   [4.2.2\. 与传统集中式工作模式的异同](http://www.worldhello.net/gotgithub/04-work-with-others/020-shared-repo.html#central-model)
        *   [4.2.3\. 合并后推送](http://www.worldhello.net/gotgithub/04-work-with-others/020-shared-repo.html#merge-and-push)
        *   [4.2.4\. 合并还是变基](http://www.worldhello.net/gotgithub/04-work-with-others/020-shared-repo.html#rebase-and-push)
    *   [4.3\. 组织和团队](http://www.worldhello.net/gotgithub/04-work-with-others/030-organization.html)
        *   [4.3.1\. 创建新组织](http://www.worldhello.net/gotgithub/04-work-with-others/030-organization.html#new-org)
        *   [4.3.2\. 组织管理](http://www.worldhello.net/gotgithub/04-work-with-others/030-organization.html#org-settings)
        *   [4.3.3\. 版本库管理](http://www.worldhello.net/gotgithub/04-work-with-others/030-organization.html#org-repo-mgmt)
        *   [4.3.4\. 个人还是组织](http://www.worldhello.net/gotgithub/04-work-with-others/030-organization.html#pros-of-org)
    *   [4.4\. 代码评注](http://www.worldhello.net/gotgithub/04-work-with-others/040-code-review.html)
        *   [4.4.1\. 提交评注](http://www.worldhello.net/gotgithub/04-work-with-others/040-code-review.html#commit-comments)
        *   [4.4.2\. 逐行评注](http://www.worldhello.net/gotgithub/04-work-with-others/040-code-review.html#line-comments)
    *   [4.5\. 缺陷跟踪](http://www.worldhello.net/gotgithub/04-work-with-others/050-issue.html)
        *   [4.5.1\. 标签](http://www.worldhello.net/gotgithub/04-work-with-others/050-issue.html#labels)
        *   [4.5.2\. 里程碑](http://www.worldhello.net/gotgithub/04-work-with-others/050-issue.html#milestone)
        *   [4.5.3\. Issue的生命周期](http://www.worldhello.net/gotgithub/04-work-with-others/050-issue.html#issue)
        *   [4.5.4\. Pull Requst也是Issue](http://www.worldhello.net/gotgithub/04-work-with-others/050-issue.html#pull-requstissue)
    *   [4.6\. 维基](http://www.worldhello.net/gotgithub/04-work-with-others/060-wiki.html)
        *   [4.6.1\. 维基初始化](http://www.worldhello.net/gotgithub/04-work-with-others/060-wiki.html#wiki-init)
        *   [4.6.2\. 使用维基](http://www.worldhello.net/gotgithub/04-work-with-others/060-wiki.html#use-wiki)
        *   [4.6.3\. 维基与Git](http://www.worldhello.net/gotgithub/04-work-with-others/060-wiki.html#git)
*   [5\. 付费服务](http://www.worldhello.net/gotgithub/05-commercial-github/index.html)
    *   [5.1\. GitHub收费方案](http://www.worldhello.net/gotgithub/05-commercial-github/non-free-plans.html)
    *   [5.2\. GitHub企业版](http://www.worldhello.net/gotgithub/05-commercial-github/github-enterprise.html)
*   [6\. GitHub副产品](http://www.worldhello.net/gotgithub/06-side-projects/index.html)
    *   [6.1\. GitHub:Gist](http://www.worldhello.net/gotgithub/06-side-projects/gist.html)
        *   [6.1.1\. 数据的粘贴和引用](http://www.worldhello.net/gotgithub/06-side-projects/gist.html#paste)
        *   [6.1.2\. Gist背后的Git库](http://www.worldhello.net/gotgithub/06-side-projects/gist.html#gistgit)
        *   [6.1.3\. Greasemonkey](http://www.worldhello.net/gotgithub/06-side-projects/gist.html#greasemonkey)
        *   [6.1.4\. 命令行操作Gist](http://www.worldhello.net/gotgithub/06-side-projects/gist.html#gist-cli)
    *   [6.2\. 其他版本控制工具支持](http://www.worldhello.net/gotgithub/06-side-projects/other-scm.html)
        *   [6.2.1\. 用SVN操作GitHub](http://www.worldhello.net/gotgithub/06-side-projects/svn.html)
        *   [6.2.2\. 用Hg操作GitHub](http://www.worldhello.net/gotgithub/06-side-projects/hg-git.html)
    *   [6.3\. 客户端工具](http://www.worldhello.net/gotgithub/06-side-projects/tools.html)
        *   [6.3.1\. github:mac](http://www.worldhello.net/gotgithub/06-side-projects/github-mac.html)
        *   [6.3.2\. hub](http://www.worldhello.net/gotgithub/06-side-projects/hub.html)
        *   [6.3.3\. iOS应用](http://www.worldhello.net/gotgithub/06-side-projects/ios.html)
    *   [6.4\. 其他](http://www.worldhello.net/gotgithub/06-side-projects/others.html)
        *   [6.4.1\. GitHub:Jobs](http://www.worldhello.net/gotgithub/06-side-projects/jobs.html)
        *   [6.4.2\. GitHub:Shop](http://www.worldhello.net/gotgithub/06-side-projects/shop.html)
        *   [6.4.3\. GitHub短网址服务](http://www.worldhello.net/gotgithub/06-side-projects/short-url.html)
        *   [6.4.4\. GitHub Open Source](http://www.worldhello.net/gotgithub/06-side-projects/opensource.html)
*   [7\. 附录：轻量级标记语言](http://www.worldhello.net/gotgithub/appendix/markups.html)

</div>

</div>

<div>

## 贡献者列表[¶](http://www.worldhello.net/gotgithub/#id7 "永久链接至标题")

Git和GitHub促进了开源软件的发展是因为消除了核心开发者和贡献者的隔阂——你若能看到代码，你就能改进代码。开放的电子书亦是如此，下面的贡献者让本书变得更好。

以贡献时间为序，感谢：

1.  [Zhang Hailong](https://github.com/zhhailon) 报告文字错误。问题： [#2](https://github.com/gotgit/gotgithub/issues/2) 。
2.  [Riku](https://github.com/riku) 纠正文字错误。提交： [455d0db](https://github.com/gotgit/gotgithub/commit/455d0db) , [f244e3d](https://github.com/gotgit/gotgithub/commit/f244e3d) 。
3.  [windwiny](https://github.com/windwiny) 纠正文字错误。提交： [1ed1a51](https://github.com/gotgit/gotgithub/commit/1ed1a51)

</div>

</div>

</div>

</div>

</div>

</div>

</div>

</div>

</div>