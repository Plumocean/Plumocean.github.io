---

title: 非天然氨基酸
description: Noncanonical amino acids
slug: ncAA
date: 2023-08-02 00:00:00+0000
image: 
categories:
    - DNA
    - Protein Labling
# tags:
#     - Tag

# links:
#   - title: GitHub
#     description: GitHub is the world's largest software development platform.
#     website: https://github.com
#     image: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
#   - title: TypeScript
#     description: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript.
#     website: https://www.typescriptlang.org
#     image: ts-logo-128.jpg



---
## 背景

生命在地球上延诞生，漫长的时间使得不同生物之间的遗传信息千差万别，但是书写这些遗传信息的语言却保持着高度的统一性，由A、G、C和T（或者U）组成，并且能够每三个作为一个翻译单元，按照几乎一样的规则翻译成组成蛋白质的20个氨基酸。

![图1：遗传密码子，OpenStax College](codon.png)

但是在一些古菌、纤毛虫甚至是线粒体中存在21或者22种氨基酸，而这些额外的氨基酸的引入也需要一些额外的与之对应的密码子、tRNA以及对应的氨酰tRNA合成酶。比如UGA在大多是生物中作为终止密码子标志着蛋白质的翻译停止，在某些生物中UGA则能够被理解为硒代半胱氨酸的编码。

对于密码子的选择有两种方式，一种是选择在正常生物中不负责编码蛋白质的终止密码子，目前最常用的是琥珀密码子UAG，因为UAG是终止密码子中出现率较低的一个，因而较常使用[^1]。而另一种被称之为移位密码子，是在原始的三位密码子的基础之上增加一到两个碱基，称之为四联体密码子或者五联体密码子，从而实现了更高的灵活性，以及对于宿主内源tRNA的竞争性识别也会更弱[^2]。

[^1]:https://www.science.org/doi/10.1126/science.2649980
[^2]:https://chemistry-europe.onlinelibrary.wiley.com/doi/10.1002/cbic.201402104

## 筛选氨基酸-tRNA-氨酰tRNA合成酶正交组

对于正交体系的设计不只是特异性密码子的设计，为希望引入的非天然氨基酸具有着天然氨基酸所不具有的功能基团，因而如何筛选出能将非天然氨基酸和对应的tRNA催化合成对应的氨酰tRNA（aminoacyl-tRNA synthetase，aaRS）才是该系统能够发挥功能的关键[^3]。

[^3]:https://pubs.acs.org/doi/10.1021/acschembio.7b00974

但是现存的氨基酸-tRNA组合都是在漫长的生物进化过程中进化所得，因而想要完全de-novo地设计出一对与目的宿主内翻译体系正交的aaRS-tRNA正交的作用过于复杂与困难了，而选择与之亲缘关系较远的物种中现存的氨酰合成酶，在此基础之上进行优化和筛选，该过程就能简化许多，第一对正交的aaRS-t
RNA就是通过在天然的基础上筛选得到，也就是第21中用于蛋白质合成的氨基酸——硒代半胱氨酸。

之后接着人们就从巴氏甲烷八叠球菌里发现了天然编码的吡咯赖氨酸，人们在解析它的某个蛋白质结构时，发现有一个与已知的氨基酸不同的种类，后来发现是一种天然编码的氨基酸——吡咯赖氨酸，对应的密码子恰巧为多数生物中最不常见的终止密码子，即琥珀密码子UAG。随后便尝试了这对aaRS-tRNA体系能否在别的生物中进行同样的翻译，或许由于该物种在进化的道路上与许多物种早早地分离开来，这套体系不需要额外的优化改造就能保持良好的正交性，由于其aaRS中与吡咯赖氨酸结合的口袋空间限制性不大，一个与之对应的文库也随之建立起来，用于引入更多与吡咯赖氨酸类似的非天然氨基酸。

![图2：筛选正交aaRS–tRNA[^4]](pipeline.png)

[^4]:https://www.nature.com/articles/s41587-020-0479-2

而如果打算更自由地创造一些正交翻译体系，定向进化在筛选特异性强的正交体系中起到了不可或缺的重要作用，在筛选正交体系过程中，首先通过结构分析aaRS的活性位点，选择拟进行突变的氨基酸残基，然后进行饱和突变以生成对应的文库。第一轮正向筛选是将非天然氨基酸插入抗生素抗性的蛋白质中，这样只有能够识别和氨酰化对应的非天然氨基酸的体系才能够存活，保证了对于非天然氨基酸密码子的识别能力；第二轮反向筛选，将非天然氨基酸密码子插入致死蛋白，但是不提供非天然氨基酸的底物，这样如果不具有较强的正交性，内源氨基酸插入到致死蛋白，从而无法存活，存活下来的保证了与天然氨基酸的正交性。

囿于分裂速度和培养条件，定向进化被选择在大肠杆菌[^5]和酵母菌[^6]中来完成，前提是在大肠杆菌和酵母菌中aaRS的正交性和哺乳细胞中的正交性相同。

[^5]:https://linkinghub.elsevier.com/retrieve/pii/S0006-291X(08)00860-7
[^6]:https://www.nature.com/articles/nmeth1016

## 非天然氨基酸系统的应用

非天然氨基酸系统能够特异性地在氨基酸的特定位点引入特异的集团，特异性强、对蛋白结构扰动小，种种优点使得该系统在药物研发、蛋白检测和生物传感器等方面都有所应用。

因为非天然氨基酸R基的多样性，引入特定的R基即可以使得蛋白质具有非天然的理化性质和功能。引入催化基团可以表现出明显优化的催化效率，引入氟相关的基团可极大提高蛋白的耐热性能，引入一些具有荧光能力的氨基酸即可避免融合荧光蛋白所带来的大空间位组和折叠错误的问题。

更进一步的，引入的非天然氨基酸可以作为进一步化学修饰的基础位点，通过点击化学或者催化偶联来引入更大的分子基团，比如聚乙二醇（Poly ethylene glycol，PEG）可以改善药物的药代参数，与多聚糖偶联来形成网状结构，或者偶联药物来合成抗体药物偶联物（Antibody-drug conjugate，ADC）。
