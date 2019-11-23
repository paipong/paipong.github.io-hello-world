# GitHub 指南

原文地址：[GitHub官网指南](https://guides.github.com/activities/hello-world/)

## 示例项目：Hello World

十分钟轻松教学

在学习计算机语言编程的过程中创建Hello World 项目是一个历史悠久的传统。当你接触一门新事物的时候可以用它来做一个简单的练习。让我们开始使用github吧！

**通过本文，您将会学到：**

>1. 如何创建和使用仓库
>2. 如何创建和管理分支
>3. 如何改变一个文件并将它提交到github上
>4. 如何发起以及合并请求

## 什么是GitHub?

GitHub是一个代码版本控制和协作的托管平台。它可以让你和你的伙伴在任何地方一起进行项目开发。

本教程将帮助你学习GitHub的必备知识，如“仓库”、“分支”、“提交代码”以及“请求代码合并”。你将创建你自己的“hello-world”仓库并且学习GitHub的请求代码合并工作流，这是目前一种非常流行的创建和审查代码方式。

**无需编码**

要完成本教程，您需要注册一个GitHub账户并且需要联网。你不需要知道如何编码，如何使用命令窗口以及如何安装Git(GitHub的客户端软件)。

提示：你可以将本指南在一个单独的浏览器或浏览器tab窗口中打开，这样你就可以边看着指南边进行操作了。

### 第一步：创建一个仓库

一个仓库通常用来组织一个单独的项目。该仓库可以包含你项目中的所有文件，如文件夹、文件、图片、视频、电子表格、数据集等。我们建议包含一个README文件，或者你自定义的用来记录项目信息的文件。GitHub将默认在你创建仓库的时候添加它。在创建的同时还提供了权限许可选项。

你可以用你的“hello-world”仓库来存储你的想法、资源，甚至用它来和别人分享、讨论任何事情。

#### 创建一个新的仓库

1. 在页面的最右上角，你的头像的左边，点击“＋”，在弹出的下拉选项中选择“New repository”。
2. 在仓库名称输入框中输入你的仓库名称：“hello-world”。
3. 写一个简短的描述。
4. 勾选“Initialize this repository with a README”。

![](https://guides.github.com/activities/hello-world/create-new-repo.png)

点击“Create repository”按钮，完成创建。

#### 第二步：创建一个分支

分支是一个可以让你在同一时间工作在同一个仓库的不同版本的方法。

在你的仓库中会有一个默认的名叫“master”的主分支，该分支用来存储你最终确定的版本代码。我们用其他的子分支来进行编辑和更改，确定之后再提交到主分支。

当你从主分支创建出一个子分支的那一刻，其实你就是对当时时间点的主分支做了一个拷贝。如果之后别的分支的人对主分支做出了更新，在你提交到主分支之前，你必须先从主分支上拉取那些更新。

下面的图表将显示分支合作的整个流程：

- 主分支
- 一个新的命名为“feature”的子分支（因为我们正在这个分支上做开发）
- “feature”分支合并到主分支之前的历程
![](https://guides.github.com/activities/hello-world/branching.png)

你是否像下面这样保存过不同版本的文件？

- story.txt
- story-joe-edit.txt
- story-joe-edit-reviewed.txt

在GItHub仓库中的分支就是为了完成类似的功能。

在GitHub上，我们的开发人员，编辑人员以及设计人员，分别在独立的分支上完成自己修改bug或功能编写的工作。当一个功能编写确定之后，他们就将自己的分支合并到主分支上。

#### 新建一个子分支

1. 进入你的“hello-world”仓库
2. 点击文件列表上方的写着“branch: master”的下拉框
3. 在输入框中输入新的分支名字“readme-edits”
4. 点击下方蓝色背景的分支创建框或直接按键盘的“Enter”键

![](https://guides.github.com/activities/hello-world/readme-edits.gif)

现在，你已经有了“master”和“readme-edits”两个分支了。他们看起来几乎一模一样，但是不要着急，接下来，我们将在我们新建的子分支上做出一些改变。

#### 第三步：做出修改并提交

干得好！现在，你已经在你的新分支“readme-edits”上了，让我们来对它写点什么。

在GitHub中，保存更改被称为“提交”。每一次提交都需要写一段我们为什么做出修改的备注说明。这些备注说明将对你的更改做出记录，其他伙伴看到之后就知道你每次都提交了什么。

**做出修改并提交**

1. 点击“README.md”文件，切换到“README.md”内容页面
2. 点击编辑框右上角的铅笔按钮，进入编辑界面
3. 在编辑框中，写一些你自己的信息
4. 在下方的“提交更改”框中，输入你做出此次修改的备注说明
5. 点击下方的“Commit changes”按钮

![](https://guides.github.com/activities/hello-world/commit.png)

这些更改只是针对于位于你的“readme-edits”子分支中的 “README.md ”文件，所以现在这个分支上包含的内容和主分支上已经有所不同。

####第四步：发出“请求代码合并”请求

现在你已经对你的新分支做出了修改，我们可以发出“请求代码合并”的请求啦。

请求代码合并是GitHub团队协作的核心功能。当你发出一个“请求代码合并”请求的时候，相当于你请求别人拷贝你当前的代码做出审查，审查通过之后将你的代码下载并且合并到他们的分支上。该请求将会在所有的分支上显示出不相同的部分。你做出的任何更改、增加以及减少，都会用绿色和红色显示出来。

在你的代码完成之前，你可以随时进行代码提交，发起请求代码合并的请求以及进行一场讨论。

你可以通过GitHub的“@”功能，在每次发出“请求代码合并”请求的时候，向特定的人或团队做出反馈，无论这个人是在你身边还是远在千里之外。

你可以向自己的仓库发出“请求代码合并”的请求，并且自己去合并他们。这在你接触到大型项目之前是一个非常好的练习方法。

**为更改的README文件发出“请求代码合并”请求**

第一步：点击“Pull Request”选项卡按钮，切换到请求代码合并页面，点击绿色的“New pull request”按钮

![](https://guides.github.com/activities/hello-world/pr-tab.gif)

第二步：选择你创建的“readme-edits”分支，与主分支进行比较。

![](https://guides.github.com/activities/hello-world/pick-branch.png)

第三步：在对比页面查看这些更改，确定他们就是你想要提交的。

![](https://guides.github.com/activities/hello-world/diff.png)

第四步：当你确定这些更改就是你所要的时候，点击绿色的“Create Pull Request”按钮。

![](https://guides.github.com/activities/hello-world/create-pr.png)

第五步：为你的更改做一个简单的标题和描述。

![](https://guides.github.com/activities/hello-world/pr-form.png)

当你写完备注描述之后，点击“Create pull request”按钮。

>**提示：**你可以使用emoji表情或者拖拽图片到评论窗口进行评论。

#### 第五步：合并你的“请求代码合并”请求

这是整个过程的最后一步，是时候将你在子分支“readme-edits”做出的更改合并到主分支“master”上了。

1. 点击绿色的“Merge pull request”按钮，将这些修改合并到主分支
2. 点击“Confirm merge”按钮
3. 由于这个分支的更改已经被合并了，所以我们还需要点击紫色框中的“Delete branch”按钮，删除这个分支

![](https://guides.github.com/activities/hello-world/merge-button.png)

![](https://guides.github.com/activities/hello-world/delete-button.png)


大功告成，你已经学会如何在github官网上管理自己的项目了。

