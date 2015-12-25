# GitTest
这是一个Git在Android Studio 、Intellij IDEA中应用的例子，主要是使用内置的Git整合的插件

远程编辑过的文件
远程编辑过的文件
## **场景一：clone一个项目**

* step1：在Github上创建一个项目``` GitTest ```

    操作如下图所示

    ![](/Images/创建项目.png)

    在github上的项目如下：

    ![](/Images/创建项目1.png)


* step2：clone该项目

    选择菜单：``` File/New/Project from Version Control/Github ```

    ![](/Images/clone项目.png)

    填写远端仓库地址：``` https://github.com/lyt1025/GitTest.git```

    ![](/Images/clone项目1.png)

    点击``` clone ```就可完成克隆项目


 ## **场景二：创建分支**
 > 从远端clone 一项目的源代码之后请记得创建分支，以免当多人协作的时候有人将代码修改并提交到远程之后，同时本地的代码也被自己修改了，这样对以后代码合并带来困扰，
 最合适的方式是：clone完之后，创建一个``` Dev分支```。然后在``` Dev分支```中进行开发，当完成某项功能开发之后，
 先从```远程的master分支```中```full```下拉远程的代码到```本地的master```，然后将```Dev分支```和```本地的master ```进行
 合并操作，最后将```本地的master 分支push```推送到远程。

   创建本地开发分支Dev的操作如下：

   * 点击New Branch创建分支

    ![](/Images/创建Dev分支.png)

   * 填写分支名称

    ![](/Images/创建Dev分支1.png)

    当创建分支完成之后，会自动切换到Dev分支。

## **应用场景三：提交代码**（Dev分支）

   * 创建要提交的文件

   创建文件夹``` File```，并在该文件下创建文件```devfile1.txt```,填写一些说明文字

   * 先进行```add```操作，点击add之后为文件名称从红色变成绿色

   ![](/Images/add操作.png)

   * 提交文件到```Dev```分支中

   ![](/Images/提交1.png)

   填写提交信息进行代码提交

   ![](/Images/提交2.png)

   点击``` commit```按钮提交代码，提交完成后文件名称由绿色变成黑色。提交完成。

## **应用场景四：将代码推送到远程的master分支**


   场景二已经提过了，在代码提交前先对本地master进行pull操作，然后再跟本地Dev分支合并

   * step 1：full下拉远程master文件，我们在github上修改一下远程代码（新建文件、修改文件）
   这里新建了一个```远程新添加的文件```文件，并且修改了文件```readMe```,如下图

   点击New File 添加文件

    ![](/Images/远程添加文件.png)

    点击编辑文件

    ![](/Images/远程编辑文件.png)

    编辑并且提交文件

    ![](/Images/远程编辑文件1.png)










