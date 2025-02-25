# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm508职业高中智慧作业试题系统设计+jsp

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1t58veLEnL?p=106)


# 研究背景与现状
时代的进步使人们的生活实现了部分自动化，由最初的全手动办公已转向手动+自动相结合的方式。比如各种办公系统、智能电子电器的出现，都为人们生活的享受提供帮助。采用新型的自动化方式可以减少手动的办公时间，增加正确率从而增加人们的幸福指数。时代进步中计算机技术的发展尤为突出，渗透进生活的方方面面，各种App、	网站、管理系统、小程序迅速占领市场。

对于学生的作业管理问题，大多数学校采用由班委收集学生作业然后上交或者通过在线直接发送到老师电脑上的方式，这类方式对于信息的发布和流程、后续的资料整理工作都是非常大的挑战。出错情况也相对明显，非常不利用学生的作业批改。对于考试而言，传统方式更为复杂，需要老师手动组织试卷并完成批改，现实学生作业试题管理中缺少一种更为优质、简单的方法途径。
## 1.2课题实现目的和研究意义
时代的发展也为人们提出了更高的要求，只有不断的学习和发展才可以前进。目前我们正在科技和网络发展的关键点，网络已实现普及。然而还是有大量的企业、机构采用传统的办公方式进行处理事务，当然传统的方式对于小规模的企业、机构来说更为适合，但想要发展就需要以发展的目光来看待问题。如果可以采用更科学、省力的方式进行办公将会带来变革。

学生的作业试题关系着学生的知识掌握水平。老师对学生的作业试题要严格把关，更要考虑到学生的作业试题质量。以往都是由学生线下自主上交作业、试卷，学生占主导地位，学校审核力度不好把控，监督不了学生的作业质量。如果采用共享的平台，把学生、教师、管理员都结合到一起，起到共同监管的目的就可以解决这类问题。学习的所有相关信息都可以由管理员直接管理，学生的学习进程也可由相关老师负责把控，把学生的作业提交工作实现流程化、清晰化，减少暗箱操作，提供更为透明的工作流程，实现学生作业试题管理的真正价值。
## 1.3课题研究内容
`　　`本系统从学生作业试题管理的工作出发，包括管理员、教师、学生三种权限。管理员的功能为学生管理、个人中心、教师管理、班级管理、作业信息管理、作业提交管理、作业批改管理，实现系统里用户的全面管控，教师的功能为发布作业、批改作业、发布试题、组成试卷、管理学生的考试信息，学生的功能为个人资料管理、在线考试、作业提交、作业管理、考试管理等。三种权限的用户功能相辅相成，不可缺少，共同帮助学生的作业试题管理。
## 1.4论文结构安排
本篇论文的结构分为摘要、目录、正文部分、总结、致谢和参考文献。正文部分为核心。正文部分分为：

第1章绪论，从课题的开发背景、现状、目的意义等进行本课题的介绍；

第2章系统分析，从系统的开发技术、环境、可行性、操作流程等进行系统的详细分析；

第3章系统设计，从系统的功能图、数据库设计、ER图、数据库表进行系统的设计；

第4章系统实现，主要介绍系统的实现界面和实现内容；

第5章系统测试，讲解主要功能的测试过程以及测试结果。








第2章 系统分析
## 2.1系统开发中使用相关技术介绍
### 2.1.1Java介绍
Java语言是从C++进行衍生出来的一种新型编程语言，他保留了c++语言中很多核心技术，继承了他的面向对象的优点，而且舍弃了很多缺点，比如在Java语言中去掉了指针，这样可以减少很多错误，还去掉了运算符，这样提高了运行处理效率。还增加了很多优点，添加了垃圾回收功能，提高了代码的使用率，总体来说，Java语言是一个分布式的、高性能的、多线程的开发语言。Java从开发之初就是打算作为一个开放性的语言技术，这就要求需要有很高的兼容性，首先就需要同样的代码程序可以在不同的计算机上运行，还要支持不同的网络，同时还要注重安全性，方便用户使用。Java语言最突出的特点就是面向对象，可以把一个对象当成很多代码状态的物体，然后进行自定义类型进行关联操作，这样进行集合起来的代码就叫对象，面向对象的方法可以使设计根据的简单，方便管理，还可以减少失败。C++最大的一个缺点就是没有垃圾回收机制，通常在编程的过程中，初始化对象时候系统会自动分配一个内存地址，如果不需要这个对象的时候，系统不能进行自动删除和回收，这样造成了很大的内存浪费，导致系统卡顿，会让系统非常的不稳定，严重的话甚至会系统崩溃，而Java语言就是在这个基础上设置了垃圾回收机制，当一个使用过的对象没有引用的时候，系统可以自动删除，回收内存，这样就可以很好的避免了内存泄漏，保障了程序的安全，同时提高了运行效率。
### 2.1.2Mysql数据库介绍
Mysql数据库是目前比较流行的一种开源数据库，可以支持多种编译器进行在线考试，从而保证了代码的可移植性，而且支持多种操作系统有很好的跨平台性，为编程语言提供所需要的API,可以多线程同时运行，这样有效的减少了内存占用率，提高了使用效率。运行的过程中还能自动优化sql查询算法，这样使数据查询速度达到了显著的提高，而且Mysql数据库还可以作为一个独立的程序在客户端中单独使用，也可以嵌入到其他程序中搭配一起使用。Mysql数据库效率非常的高，可以处理上千万条数据，可以同时支持多种不同的数据引擎，而且是开源的软件，不需要支付任何费用，而且可以进行定制，使用GPL协议进行代码修改，开发属于自己的Mysql系统。综上所述，Mysql数据库是一个非常受欢迎的一个数据库，体积小，速度快，最重要的还是免费，非常适合中小型项目的开发使用。
### 2.1.3B/s架构介绍
B/s架构是随着网络快速发展而开发出来的一种网络框架，跟传统的cs框架最大的区别就是，直接把代码部署到网络服务器中，这样方便了系统的后期开发和维护，然后用户可以直接通过浏览器进行代码的访问，不需要额外安装任何的软件客户端，简化了用户的使用。B/s结构是指Browser／Server结构，意思就是只需要安装一个服务器就行了， 客户端方面主要就是采用浏览器进行访问，主要是对传统的c/s架构的一种改进，采用www浏览器技术和其他Script语言技术，把系统实现需要的代码全部部署到了服务器上面，是一种新型的架构技术，可以直接借助浏览器进行数据访问和数据交互。最大的优点就是，不需要安装客户端，不受环境影响，可以实时实地的进行访问，其次就是维护非常的方便。当然了有优点也有不可避免的缺点，首先是在访问速度方面，比较受网络的影响，不像C/S架构一样，处理速度非常的快，直接在本机就可以完成数据交互，而B/s需要借助网络才能进行服务器访问，必须保证有顺畅的网络，才能有好的使用体验，其次就是安全性，因为所有数据存储在网络服务器中，比较容易受到攻击，从而造成数据泄漏，这是目前B/s架构存在的最大的弊端。所以说B/s架构适合一些电子商务类的网站，适合比较有用户共享交互的，开放性的网站的设计与开发。所以本人开发本系统采用B/s架构是非常适合的，可以达到多人同时登录系统，可以实现信息交互，而且方便随时随地的进行数据访问，而且本人对B/s架构开发比较熟悉，所以本系统就采用B/s架构来进行开发设计。
## 2.2系统可行性分析
系统的可行性关系着系统开发的成功和市场，没有经过详细可行性分析的系统开发过程会非常艰难。系统可行性从系统的经济方面、操作方面和技术方面进行分析。
### 2.2.1经济可行性分析
`   `系统开发所需要的经济主要在系统的成本问题、运行问题和维护问题上。本系统在开发中不需要经济的支撑，所需要的开发软件和设备都是在已有条件上。本系统在运行里所需要的环境也都为免费就可以下载的。本系统在后期的维护上也只需要技术支持就可以完成。所以本系统在经济可行性上可以通过。
### 2.2.2操作可行性分析
`   `本系统在开发中充分调查了所使用用户的操作习惯和风格，所有的操作流程也都为简单的流程，在操作中也设置了提醒。用户在使用本系统时只要按照提示就可以完成，非常简单。所以本系统在操作可行性上可以通过。
### 2.2.3技术可行性分析
`   `本系统所需要的技术支持为Java语言，Mysql数据库，Vue技术和SSM框架等。所使用的技术都为开源成熟的技术，也是目前流行的技术之一。使用这些技术开发的系统可以保证系统的前詹性和稳定性、安全性。所以本系统在技术可性性上可以通过。
## 2.3系统需求分析
目前计算机、网络技术已进入到各行各业。学校做为人才的培养中心更应身体力行，学校里的所有工作都是围绕学生而展开，每位学生的档案信息都非常多，如果采用传统的管理方式非常容易造成混乱，而且对于学生的信息查询非常不便。对于学生的作业、试题需要额外的严谨，如果还是采用传统的学生作业、试题管理方式对学生做不到百分百的监管，学生的作业、试题完成也实现不了透明。所以非常需要新的管理方式出现。
## 2.4系统性能分析
系统在设计时也需要注意系统的性能，一般系统的性能方面包括系统的稳定性、安全性、界面设计方面、操作方面、协调等方面。

1. 本系统在界面设计方面尊重所有的使用权限，多方面参考不同使用权限的使用习惯以及风格，综合不同的情况整理出符合大众要求的系统界面。做到自己的最大能力；
1. 在系统的稳定性、安全性方面采用必要的登录验证，不同权限采用不同的账号和密码。为了使系统更为稳定采用成熟的开发环境和技术，在代码编写时尽可能的减少冗余，保证系统的运行效率；
1. 在系统的操作流程方面，尽可能的采用简单的流程来实现用户要求的反馈，当用户提出需求时，可以用最少的步骤进行提问操作；
1. 本系统采用数据库和功能界面分开设计，这样可以保证当系统的功能运行出错时不会影响系统里的数据，也就保证了数据的安全。
## 2.5系统功能分析
系统的功能分析决定了系统的功能设计，完整详细的系统功能分析可以使系统的开发事半功倍。本系统的功能围绕学生、管理员、教师三种权限设计。根据不同权限的不同需求设计出更符合用户要求的功能。本系统中管理员主要负责审核管理三种身份以及管理系统里的信息，教师负责发布试题和考试试卷、作业，学生负责在线考试和提交作业以及作业管理，教师查看学生的考试情况和完成学生的作业批改。本职业高中智慧作业试题系统管理员的用例图如下图2-1所示：

![](/md/blog.001.png)

图2-1管理员用例图

学生可以管理个人资料、提交作业、作业信息管理和在线考试等，学生用例图如下图2-2所示：

![](/md/blog.002.png)

图2-2学生用例图

教师可以管理个人资料、发布作业、管理考试信息、试卷信息、作业信息等，教师用例图如下图2-3所示：

![](/md/blog.003.png)

图2-3教师用例图
## 2.6系统操作流程分析
`　　`信息从如何产生到反馈结果的过程可以称为信息的流程。分析好系统的操作流程才可以使系统正确运行不会出现Bug。本系统的流程为管理员先进行登录，登录后管理学生、教师的账号、密码等信息。教师使用管理员设置的账号密码进行登录，然后发布作业，学生查询到作业后可以完成和提交，教师进行学生作业的批改等。本职业高中智慧作业试题系统的操作流程如下图2-4所示：

![](/md/blog.004.png) 

图2-4职业高中智慧作业试题系统操作流程图

第3章 系统设计
## 3.1系统功能结构设计
系统的功能结构是采用树形图来绘制功能设计。根据分析所得，本系统的功能设计为管理员、学生和教师三部分。管理员为角色管理，教师为发布作业、试卷、试题进行作业批改等，学生完成作业和在线考试、查看作业等。本职业高中智慧作业试题系统的功能结构设计图如下图3-1所示：

![](/md/blog.005.png)

图3-1职业高中智慧作业试题系统功能结构图
## 3.2数据库设计
`　　`数据库为数据的仓库，决定了数据的保存和修改、删除、调用等。数据库的稳定决定了系统里数据的安全。本系统采用Mysql数据库，在建立数据库时采用Root用户名。数据库的建立过程为先进行数据的ER图设计然后进行数据库表的实现。
### 3.2.1数据ER图设计
数据ER图中记录了关系、实体、属性。实体与实体的关系决定了数据在调用时的正确与否，实体的属性决定了该实体的内容。数据ER图的设计同样重要，也是数据库建立的基础。

通过系统中的功能数据分析，本系统的实体主要有教师、管理员、学生、作业、试卷等。

1. 管理员的ER图中的属性有账号、密码、权限。管理员ER图如下图3-2所示：

![](/md/blog.006.png)

图3-2管理员ER图

1. 教师的ER图里的属性有职称、姓名、编号等，教师的ER图如下图3-3所示：

![](/md/blog.007.png)

图3-3教师ER图

1. 作业的ER图里的属性有作业标题、作业内容、发布时间等，作业的ER图如下图3-4所示：

![](/md/blog.008.png)

图3-4作业ER图

(4)试题的ER图里的属性有题目、编号、答案、解析等，试题ER图如下图3-5所示：

![](/md/blog.009.png)

图3-5试题ER图

（5）试卷ER图里的属性有试卷编号、试卷题目、答案、试卷类型等，试卷ER图如下图3-6所示：

![](/md/blog.010.png)

图3-6试卷ER图

（6）系统关系ER 图如下图3-7所示：

![](/md/blog.011.png)

图3-7系统关系ER图
### 3.2.2数据库表设计
数据库表是把ER图进行详细化、实体化。不同的表名下保存着相对应的表信息数据。在数据库表里记录着数据的主键、外键、数据类型、长度等。本职业高中智慧作业试题系统所创建的数据库表有管理员信息表、教师信息表、学生信息表、作业信息表、试卷信息表等。本职业高中智慧作业试题系统的数据库表如下表3-1—3-12所示：

表3-1 banji

![](/md/blog.012.png)


表3-2 config

![](/md/blog.013.png)

表3-3 exampaper

![](/md/blog.014.png)

表3-4 examquestion

![](/md/blog.015.png)





表3-5 examrecord

![](/md/blog.016.png)

表3-6 jiaoshi

![](/md/blog.017.png)





表3-7 token

![](/md/blog.018.png)

表3-8 users

![](/md/blog.019.png)

表3-9 xuesheng

![](/md/blog.020.png)



表3-10 zuoyepigai

![](/md/blog.021.png)

表3-11 zuoyetijiao

![](/md/blog.022.png)


表3-12 zuoyexinxi

![](/md/blog.023.png)




















第4章 系统详细实现                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
## 4.1用户登录功能的详细实现
用户登录界面起到验证身份的作用，本界面采用图片背景进行设计。在用户登录界面里设置了程序的名称和用户、密码、权限的文本框。在文本框下是登录按钮、学生注册按钮。用户在信息输入完成后可以使用相应按钮进行相对应的操作。用户登录功能的实现界面如下图4-1所示：

![](/md/blog.024.png)

图4-1用户登录实现界面
## 4.2管理员权限的功能实现
### 4.2.1个人中心管理功能的详细实现
`   `个人中心管理功能的作用为修改密码和添加、删除管理员用户。本功能可以实现新增管理员和减少管理员。个人中心管理功能的实现界面如下图4-2所示：

![](/md/blog.025.png)

图4-2个人中心管理功能的界面实现
### 4.2.2学生信息管理功能的详细实现
管理员负责学生信息的录入和管理，学生的账号和密码则是由本功能进行添加。管理员查询学生信息的功能实现如下图4-3所示：

![](/md/blog.026.png)

图4-3管理员查询学生信息的实现界面
### 4.2.3教师管理功能的详细实现
管理员可以对教师的信息进行管理、审核。同样，教师的账号和密码是此功能进行录入的。管理员查询教师信息的实现界面如下图4-4所示：

![](/md/blog.027.png)

图4-4管理员查询教师信息的实现界面
### 4.2.4班级管理功能的界面实现
`　　`管理员可以添加和查询、修改班级的功能，班级可以更好的统计学生资料。班级查询功能的实现界面如下图4-5所示：

![](/md/blog.028.png)

图4-5查询班级信息功能的实现界面
### 4.2.5作业信息管理功能的实现界面
管理员可以对作业进行下载、查询和修改等操作，还可以添加作业信息。管理员查询作业信息的实现界面如下图4-6所示：

![](/md/blog.029.png)

图4-6管理员查询作业信息的实现界面
### 4.2.6作业提交管理功能的实现界面
管理员可以查询学生提交的作业并进行修改、删除等操作。管理员查询作业提交功能的实现界面如下图4-7所示：

![](/md/blog.030.png)

图4-7作业提交功能的实现界面
### 4.2.7作业批改功能的实现界面
管理员也可以查询学生的作业批改信息并对作业批改内容进行一定的修改。作业批改功能的实现界面如下图4-8所示：

![](/md/blog.031.png)

图4-8作业批改功能的实现界面
## 4.3学生权限的功能详细实现
### 4.3.1个人中心管理功能的详细界面实现
当学生登录进系统后可以修改自己的资料，可以使自己信息的保持正确性。学生个人中心管理的实现界面如下图4-9所示：

![](/md/blog.032.png)

图4-9个人中心管理功能的运行界面
### 4.3.2作业批改管理功能的详细实现
学生可以查询老师批改后的作业，并进行作业修改后再次提交。作业批改管理功能的界面实现如下图4-10所示：

![](/md/blog.033.png)

图4-10查询作业批改功能的运行界面
### 4.3.3作业提交管理功能的详细实现
学生可以浏览自己提交的所有作业信息。作业提交管理功能的实现界面如下图4-11所示：

![](/md/blog.034.png)

图4-11作业提交管理功能的运行界面
### 4.3.4作业信息管理功能的实现界面
学生可以查询作业，并完成作业提交。作业信息管理功能的实现界面如下图4-12所示：

![](/md/blog.035.png)

图4-12作业信息管理功能的实现界面
### 4.3.5考试管理功能的实现界面
学生可以查看试卷并进行在线考试和查看考试成绩以及管理错题本。实现界面如下图4-13所示：

![](/md/blog.036.png)

图4-13考试管理功能的实现界面
## 4.4教师权限的功能详细实现
教师的功能为发布试题、作业信息和试卷信息管理学生的作业和考试信息等。教师权限的功能实现界面如下图4-14所示：

![](/md/blog.037.png)

图4-14教师权限功能的运行界面
## 4.5学生注册功能的实现界面
`    `学生在登录界面里可以进行注册，注册后的资料可传送到管理员手中，在注册时需要填写密码，密码为学生在登录时需要输入的信息。学生注册功能的实现界面如下图4-15所示：

![](/md/blog.038.png)

图4-15学生注册功能的实现界面
















第5章 系统测试
# 系统测试的方










