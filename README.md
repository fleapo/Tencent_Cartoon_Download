# 腾讯漫画下载脚本

这是一个腾讯漫画的下载脚本..通过Python编写

### 目前实现的功能有:

- 通过名称查找漫画列表(目前只查找到了漫画的数目)
- 根据查找到的漫画列表显示漫画的一共有多少个章节
- 根据输入的章节索引下载漫画章节
- 下面的TODO-Next中被删除的内容已经在这次提交中实现

### 目前已测试过能完整下载的漫画有:
- [火影忍者(共711话)]
- [白灵杀手(共136话)]
- [女主播攻略(共41话)]
### 目前存在的Bug有:

- ~~当下载章节较多时,会出现远程主机被关闭的问题~~

- ~~Win与Linux路径上的规则不同导致生成的文件夹放置的位置无法放置在项目的根目录中~~

- Linux系统中存在当需要下载的章节较多时,内存占用很高,同Code下Win平台不存在此问题

- 当下载的漫画章节很多时,出现假死的状态

- Win平台下出现下载完成后无法停止的现象 Linux下正在频繁测试中(现在发现似乎也会出现Win平台的状况)

- 不知是因为我自己的网络原因还是code有问题,存在一种最开始下载很快不过后面几乎无速度的状态

- 目前的写法是有问题的.创建了一个超级大的list 但是没有释放.....这不能忍

### ToDo-Next:


- ~~实现多进程~~

- 显示出查找到漫画列表

- ~~目前下载的图片都下载到根目录中,需要生成一个文件夹来保存下载的图片~~

- 根据不同的章节生成不同的文件夹来保存

- 添加程序的守护进程

- 将下载的章节内容生成PDF供阅览

- MIT License

PS:本人是一个动漫爱好者,这只是我自己一时脑热想出来的一个想法,这里只做下载内容的东西,详细的如何通过页面中的数据获取到漫画的图片地址本人不做任何解释,当然你对此项目有任何的想法或建议可以在issue在提出,欢迎各位提出自己宝贵的意见,跪求star
