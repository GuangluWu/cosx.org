---
title: 重要的不是谁获 COPSS 奖，而是它给我们的启发和思考
date: '2019-08-06'
author: 统计之都
categories:
  - 新闻动态
tags:
  - COPSS
  - Hadley Wickham
  - RStudio
  - ggplot2
  - tidyverse
  - 统计学
forum_id: 420832
slug: copss-hadley-special-comment
---

> 编者按：在[前文](https://cosx.org/2019/08/copss-hadley-comments/)中我们刊登了收集到的各方评论。本文刊登的是统计之都邀请的一位特约评论员的长文评论。

![Hadley in COPSS](https://user-images.githubusercontent.com/1142836/62476732-2a2f3080-b7da-11e9-9c38-60556399484c.jpg)

在谈 Hadley 获奖这个问题之前，我想拿另外一件事作对比。可能统计学比较小众，它的最高奖项也不太为人所知。除了有些人头一次听说的 COPSS 奖之外，另一个最高奖项应该算是统计学国际奖（International Prize in Statistics），这个奖还比较年轻，知道的人可能更少，感兴趣的人可以参见 <https://statprize.org>。最近一次（其实也就是第二届）的获奖者是 Efron，获奖理由是他的 Bootstrap 方法。相信统计学界都已熟知他的故事；不熟的可以读一读 2003 年 Statistical Science 杂志上的采访稿，题为 Bradley Efron: A Conversation with Good Friends。简短说就是 Efron 当年把 Bootstrap 的论文投给 Annals of Statistics 杂志（所谓的“四大天王”之一甚至之首）时，被一位编辑以“这篇论文连一个数学定理都没有”为由给拒稿了。如果我们想一想 Bootstrap 这几十年来的巨大影响和广泛应用，那么我们难免觉得那位编辑短视和迂腐得可怕。那位编辑可能是觉得论文的想法太简单，普通人一眼就能看懂，所以不能发表。这想法若用 R 语言实现，其核心也是简单得不能再简单的一行代码：`sample(x, replace = TRUE)`。

今天当有人在用“码农的工作太初级、太简单、连一个数学定理都没有”来反对 Hadley 获奖的时候，我想请你静下心来想想你是不是也要像那位编辑一样枪毙 Bootstrap 方法。当我看见有人高呼 COPSS 奖万万不可颁给一个“码农”的时候，感觉就像那些不肯剪辫子的遗老一样：祖宗之法不可变啊。以往历年的 COPSS 奖全都颁给了学术界的人，然而这个奖项的规则中并没有说不能颁给工业界的人或是“码农”。它强调的是对统计学的贡献，而贡献可以是多样化的。

我是统计学科班出身（虽然本人不才，本硕博加起来花了十多年），在我读本科的时候我一心向往学术界，但上了研究生之后，我就渐渐对统计学失去了信心。这里面有多重因素，比如统计学研究生阶段花了大量时间在“中心极限定理的三种证法”和在各种嵌套得像毛线团的线性模型的方差分析表上数自由度上，而学术论文通常倾向于装腔作势把本来很简单的想法说得无比复杂（因为怕太简单被拒稿），以及Leo Breiman 的 Two Cultures 论文让我头一次开始怀疑令我们沾沾自喜的“模型可解释性”究竟是不是皇帝的新装等等。在 Hadley 这次获奖之前，我已经对“正统”统计学界完全失去了兴趣，我觉得统计学正在被快速边缘化，而圈内的人还自以为统计学王朝依然歌舞升平、碰到问题先泰勒展开再说。在学校里学到的理论都很美好，但走出校门第一步就会被绊倒：十八般武艺学了一身，而到了现实世界中，却发现用武之地需要自己徒手搭建。为什么？因为为了能让你的漂亮模型上台五分钟，你还得先在台下用十年功先把数据整理出来。统计学离开了数据还能叫统计学吗？我觉得肯定不能，而多数与数据打交道的人都知道，建模花的精力与整理脏数据相比简直是微不足道。

在我眼中，Hadley 有两项常人不具备的特殊能力。这里我说的“常人”指统计学家和码农的集合。第一项能力是将问题抽象至普通人能理解的程度，例如 `ggplot2` 将统计图形抽象为若干个可自由组合的元素、`dplyr` 将数据清理抽象为少数几个动词。这些抽象都不能算是他的绝对原创，他也是借鉴了别人或别的社区的理念。虽然这些理念存在已久（例如 *The Grammar of Graphics*、数据库中的范式、SQL 语言），但并没有人将这些理念以浅显的形式解释并实现出来，让数据工作者（我比较排斥“数据科学家”这个名词）很快就能上手使用。我认为他的这些抽象与数学定理的抽象并没有区别，我们决不能说数学的抽象就更高贵，而代码的抽象则更低贱。有人认为推公式需要极大的耐心和努力去坐冷板凳，殊不知写代码一样要坐冷板凳，去仔细考虑如何从众多不同的实际问题中抽象出一条简洁的路。有人可能质疑，为什么不颁奖给 Lee Wilkinson（*The Grammar of Graphics* 一书的作者）或者 R 语言的创始人，我觉得这种质疑没有道理，照这么说我们该颁奖给我们的电脑生产商才是。原材料是很重要，但把原材料打磨成艺术品的艺术家也有他们的特殊贡献。因为有抽象在，所以 Hadley 的工具通常有很强的组合性能，这就像 Unix 的设计哲学之一：不同的简单命令可以通过管道自由组合以完成特定的任务。如果没有抽象，你可能意识不到条形图和玫瑰图本质上一样，只不过一个用了笛卡尔坐标系，一个用了极坐标系而已；而在 ggplot2 中，变换坐标系有着同样的抽象命令，因为坐标系是图形的一个独立组成元素。 Hadley 非常擅长借鉴别的社区的抽象概念，他写代码不像普通码农，上来就直接写，而是先退到问题的本质状态，想清楚尽量普适的招式，让用户能打出一套组合拳去解决他们的数据分析问题。这种能力很值得我们借鉴和学习。对于那些认为 Hadley 沽名钓誉的人，我也不能说他们绝对没有道理。是的，伯乐是沾了千里马的光，但我们得意识到：千里马常有，而伯乐不常有。每一个行当的人都容易对自己的行业过度自信，不关心别的行当在做什么、有什么值得学习借鉴的，这是人性的弱点之一，而 Hadley 则克服了这个弱点，他可以持续寻找有用的千里马。

我得直言，Hadley 的另一项特殊能力是营销。论营销，我觉得统计学家可能是世上营销能力最差的一群人（这也很可能是我在统计学界念书时间太久而导致的心理偏误）。在我读博期间，我非常想呼吁系里的老师们建一个群博客，然而根本没有人有兴趣。论实力，我觉得我们系的老师卧虎藏龙，一定可以写出很有深度和有意思的博客文章来，但就是没有人觉得在这个时代，除了在只有自己的博士生会看的杂志上发表论文以及去 JSM 会议对着稀稀拉拉十位听众做报告之外还有其它宣传的渠道。我曾为此感到深深的失望，眼睁睁看着别人系的博客红红火火，而我们系则继续烂在玉米地里。一定程度上，Hadley 确实是走了网红的路线，这容易招致批评，包括我对此也不尽认同。按我的个人标准，他的营销有点过度，而事实是在统计学家里，他可能是粉丝最多的推特账号。统计学家可能都太实诚，不愿意自己推销自己，唯恐被人认为王婆卖瓜，但在杂志上发表论文推销自己跟在社交媒体上推销自己又有什么本质区别呢？后者比前者要高效得多。奥巴马和特朗普不就是分别靠脸书和推特当上美国总统的吗？如今我自己已经非常反社交媒体，因为那上面太嘈杂、也容易让人上瘾，但我想说的是，统计学家早需要适当提高自己的营销水平了。

说到这里，我得继续向 Hadley 的广大粉丝直言，各位千万不要搞偶像崇拜。尤其是近两年，我观察到一些极度脑残的群体偶像崇拜行为。我认为这无论是对 R 社区还是对统计社区，都是非常不健康的。这种偶像崇拜风气，与 Hadley 本人的大力营销不无关系。我不记得是去年还是前年，他发了一张自己戴着蝴蝶领结的靓照，而随后的万圣节就有过度热心的粉丝照着这张靓照刻了南瓜灯，而且蝴蝶领结（bow tie）也成了粉丝圈津津乐道的一个梗。他长得帅不帅、梳什么发型、戴什么领结、穿什么衬衫、调什么鸡尾酒、烧烤什么肉，与我们毫无关系，我们完全不需要关注。喜欢一个人的作品就好，不要延伸到一些无关的方面（如外观和生活），更不要为了这个人而参与抨击、打压他的对立者或竞争者。比如不要把他创建的所谓 `tidyverse` 搞得像传销一样（仿佛没了管道操作符就写不了 R 代码了、没了 `tibble` 就没了可用的数据类型），也不要因为 Hadley 写代码获奖而开始瞧不起统计理论工作者。若你因为码农获奖而瞧不起理论工作者，那么你就跟部分瞧不上码农的理论工作者一样自以为是。尽管长期以来，统计计算和图形研究者在统计学界都是弱势群体（尤其是图形和可视化，总入不了统计学家的法眼），但我们莫要杀死前面那条恶龙而盘踞山头成为新的恶龙去吞噬他人。

Hadley 获奖后，我建议大家不要光顾着恭喜他本人。我们真正需要感到欣喜的不是这个特定的人（他是不是 Hadley 其实没那么重要），而是统计学界尚存希望，也就是存在去除一条愚蠢的鄙视链条的希望：离实际问题同样近甚至更近的代码工作者，应该得到同样的尊重和认可；COPSS 奖的评选，总算出现了一点马尔可夫性的希望，不再年复一年陷在单纯奖励推定理的人上。

前几年孟晓犁老师把 COPSS 奖称为“统计学界的诺贝尔奖”，我觉得这种称谓不甚妥当，它让这个奖项的光环太耀眼，仿佛在塑造超级明星，容易加剧偶像崇拜。人们总需要明星的激励和引导，但人又总容易把眼光局限在明星个人身上，缺乏进一步的抽象，即：这位获奖者的哪些素质和能力值得我学习？我们不必做到“无我相”，但我觉得做到“无人相”很重要，尤其是对台上光芒万丈的获奖者（他具体是谁根本不重要）。COPSS 奖也是活人（五位统计协会的头目）选出来的，他们也许有大智慧，也许有偏颇，这个决策过程我们都不知道（有哪些候选人都不知道，也许其他厉害的人碰巧今年都没被提名）。要是你觉得有理，也用不着狂欢；要是觉得没理，也犯不着怒骂。作为统计学家，你应该对任何事情都保留一个随机误差项。要是你觉得码农获奖就确定一定以及肯定代表了这个码农比其他人都绝对强，那你可能还不是合格的统计学家。世上哪有那么多碾压群雄的一致最小方差无偏估计量（UMVUE）。所有获奖者，无非是在特定条件下的最优估计量而已，而且还只是个点估计（盯着点估计认死理的统计学家也不是合格的统计学家）。清楚这点之后，各位便可以各回各家、各找各妈，该干嘛干嘛。只要你真心认为自己的工作有意义，那工作本身就已经是你最大的奖励，何必把目光盯在那个区区 COPSS 奖上呢。
