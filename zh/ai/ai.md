# 人工智能

## 关键词
深度学习, 强化学习, 机器学习, 人工智能, 数据科学

## 说明
在自然语言生成领域，AI已经表现出了非常出色的能力，可以生成高质量的文章、故事、诗歌等。  
在对话系统领域，AI可以实现高质量的人机对话，可以应用于客服、智能助手等场景。在推荐系统领域，AI可以根据用户的历史行为和兴趣，进行个性化推荐。  
在知识图谱构建领域，AI可以用于实体识别、关系抽取、问答系统等。  
在智能家居领域，AI可以实现更加智能化的家居控制，实现更加便捷舒适的生活。  
在人工智能教育领域，AI可以实现更加智能化的教育辅助，帮助学生更加高效地学习。  
在语音识别领域，AI可以实现更加准确的语音识别，可以应用于智能语音助手、语音翻译等场景。  
在机器人领域，AI可以实现更加智能化的机器人控制，可以应用于家庭服务、工业制造等场景。

## 缩略词

ACRONYM | Meaning
-------:|-------------------------------
 AI     | Artificial Intelligence
 DL     | Deep Learning
 RL     | Reinforcement Learning
 ML     | Machine Learning
 AI     | Artificial Intelligence
 NLP    | Natural Language Processing
 CNN    | Convolutional Neural Network
 SAN    | Stacked Auto-encoder Network

## 代码

```shell
python3 -m pip install datasets scipy matplotlib torch torchtext ipywidgets nltk watermark bertviz spacy networkx
python3 -m spacy download pt_core_news_sm
```

## 框架

### [PYTORCH](https://pytorch.org)
<https://github.com/pytorch>

1. [Introduction](https://pytorch.org/tutorials/beginner/basics/intro.html), [nn.Module]((https://pytorch.org/docs/stable/generated/torch.nn.Module.html), [nn.Transformer](https://pytorch.org/docs/stable/generated/torch.nn.Transformer.html), [data.DataLoader](https://pytorch.org/docs/stable/data.html), [nn.Linear](http://pytorch.org/docs/stable/generated/torch.nn.Linear.html), [nn.Embedding](https://pytorch.org/docs/stable/generated/torch.nn.Embedding.html), [nn.CrossEntropyLoss.html](https://pytorch.org/docs/stable/generated/torch.nn.CrossEntropyLoss.html)
2. [PyTorch 数据处理教程(1)      ](https://zhuanlan.zhihu.com/p/448064320): <https://learn.microsoft.com/en-us/training/modules/intro-machine-learning-pytorch/4-model>
3. [Torchtext Field新版本中被移除](https://zhuanlan.zhihu.com/p/485686510): `python3 -m pip install torch==1.9.0 torchtext==0.10.0`, <https://github.com/pytorch/text/blob/master/examples/legacy_tutorial/migration_tutorial.ipynb>

### [百度飞桨](https://www.paddlepaddle.org.cn)

### [OLLAMA](https://ollama.com)
Mirror: <https://ollama.org.cn>

Begginer: [Ollama 本地运行大模型(LLM)完全指南](https://blog.csdn.net/2401_85390073/article/details/144569533)

Chatbox, [Dify知识库](https://github.com/langgenius/dify.git)

### [Huggingface](https://huggingface.co)

Mirror: <https://hf-mirror.com>

#### [datasets](https://huggingface.co/docs/datasets)

`datasets.load_dataset("csv", data_files="my_file.csv")`  
`datasets.load_dataset("text", data_files="my_file.txt")`  
`datasets.load_dataset("json", data_files="my_file.json")`  
`datasets.load_dataset("pandas", data_files="my_file.pkl")`

`data_files` can be either a single file path, a list of file paths, a dictionary that maps split names to file path, blob files like unix shell, url to remote file

`datasets.Dataset.unique`, `datasets.Dataset.shuffle`, `datasets.Dataset.select`, `datasets.Dataset.sort`, `datasets.Dataset.add_column`, `datasets.Dataset.train_test_split`, `datasets.Dataset.to_json`, `datasets.Dataset.to_csv`

`dataset.load_dataset("csv", data_files="my_file.csv")["train"].shuffle(seed=10).select(range(10))` where shuffle will randomly select data but seed will make result consistent, select will select the list of data.  
`dataset.load_dataset("csv", data_files="my_file.csv")["train"].unique("column name")` can return unique data  

`datasets.DatasetDict.rename_column`, `datasets.DatasetDict.map`,  `datasets.DatasetDict.filter`,  `datasets.DatasetDict.set_format`,  `datasets.DatasetDict.reset_format`,  `datasets.DatasetDict.save_to_disk`,  `datasets.load_from_disk`

`dataset.load_dataset("csv", data_files="my_file.csv").map(lambda x: {'normal_data': html.unescape(x['html_data'])}, batched=True)`

#### [Transformers](https://huggingface.co/docs/transformers)

`tokenizer = transformers.AutoTokenizer.from_pretrained('bert-base-cased')`

1. <https://github.com/huggingface/transformers>

## Repositories
1.  <https://github.com/topics/machine-learning>
2.  <https://github.com/project-baize/baize>
3.  <https://github.com/intel/openfl>: `pip install openfl, docker pull intel/openfl`
4.  <https://github.com/facebookresearch/llama>
5.  <https://github.com/microsoft/sample-app-aoai-chatGPT>
6.  <https://github.com/Dao-AILab/flash-attention>
7.  <https://github.com/xai-org/grok-1>
8.  <https://github.com/hpcaitech/Open-Sora>
9.  <https://github.com/DataForScience/ChatGPT>
10. <https://github.com/Azure-Samples/azure-search-openai-demo>
11. <https://github.com/lencx/ChatGPT>
12. <https://github.com/mlabonne/llm-course>

1. <https://huggingface.co/spaces/project-baize/baize-lora-7B>

## 书单
1.  [李航. 统计学习方法. 清华大学出版社                          ](https://zhuanlan.zhihu.com/p/599249709)
2.  [李航老师《统计学习方法》及相关资源（代码、课件）的汇总及下载](https://blog.csdn.net/master_Shen/article/details/121354650)

3.  [机器学习实战 人民邮电出版社               ](https://www.mr-wu.cn/machine-learning-in-action-free-ebook)
4.  [机器学习实战 微信读书                     ](https://weread.qq.com/web/reader/3a232380718ff63f3a281acke4d32d5015e4da3b7fbb1fa)

5.  [《机器学习》周志华 PDF 下载                                 ](https://zhuanlan.zhihu.com/p/594408532)：含百度网盘下载链接
6.  [周志华. 机器学习. 清华大学出版社                            ](https://www.zhihu.com/question/39945249): 作为入门书，不够详尽。作为工具书，不够深入。作为科普书，不够友好。可作为教科书。
7.  [北大新书教材推荐《最优化：建模、算法与理论》](https://zhuanlan.zhihu.com/p/364637287)
8.  [最优化：建模、算法与理论](http://faculty.bicmr.pku.edu.cn/~wenzw/optbook/opt1.pdf)
9.  [邱锡鹏. 神经网络与深度学习. 机械工业出版社                  ](https://nndl.github.io)
10. [《回归分析及其试验设计》华东师范大学出版社                  ]

11. [<<机器翻译统计建模与深度学习方法>>](https://github.com/NiuTrans/MTBook), [<<机器翻译统计建模与深度学习方法>>](https://opensource.niutrans.com/mtbook)

12. [Machine Learning in Action](https://www.manning.com/books/machine-learning-in-action): [`Source Code`](https://www.manning.com/downloads/1108)

13. [Deep Learning](https://www.deeplearningbook.org): <https://github.com/exacity/deeplearningbook-chinese>, <https://github.com/daviddao/deep-learning-book/blob/master/DeepLearningBook.pdf>

14. [开源项目与评测](https://opensource.niutrans.com/mtbook/section1-7.html)

### 阅读中
1. 机器学习实战
2. 最优化：建模、算法与理论

## 参考
1. [Logit详细解释](https://zhuanlan.zhihu.com/p/27188729)
2. [Logistic回归和梯度上升算法](https://blog.csdn.net/whai362/article/details/51860379)

3. [局部加权回归（Lowess）](https://www.jianshu.com/p/1ab48eebd2a0)

4. [L0范数及数据压缩感知](https://zhuanlan.zhihu.com/p/496202983)

5. [主成分分析实现数据描述与变量压缩(附 Python code 与源数据)](https://zhuanlan.zhihu.com/p/193116314)

6. [Transformer模型详解（图解最完整版）](https://zhuanlan.zhihu.com/p/338817680)

7. [支持向量机（SVM）——原理篇](https://zhuanlan.zhihu.com/p/31886934)

8. [《机器学习》周志华 PDF 下载](https://zhuanlan.zhihu.com/p/594408532)

9. [AIGC](https://baike.baidu.com/item/AIGC/59988381)

10. [AIGC元年，全球巨头进入人工智能决赛圈？](https://www.jiemian.com/article/8757519.html): AI绘图工具Midjourney, OpenAI发布聊天机器人模型ChatGPT
11. [AIGC，喊出了元宇宙的“芝麻开门” ](https://www.sohu.com/a/630451347_121070048)

12. [DALL·E 2](https://openai.com/dall-e-2/#demos)
13. [AIGC产业链全梳理](https://zhuanlan.zhihu.com/p/584419740)

14. [MOSS and ChatGPT](https://www.infoq.cn/article/Ag3vW0mgvdd9BKyWx1iO)

15. [OpenAI](https://openai.com)

16. [ChatGPT 的起源](https://www.sohu.com/a/662849294_121679003)
17. [用ChatGPT训练羊驼：「白泽」开源，轻松构建专属模型，可在线试玩](https://finance.sina.cn/tech/2023-04-04/detail-imypfhpc2954166.d.html), <https://huggingface.co/spaces/project-baize/chat-with-baize>, <https://github.com/project-baize/baize-chatbot/blob/main/README.md>
18. [《Baize: An Open-Source Chat Model with Parameter-Efficient Tuning on Self-Chat Data》](https://arxiv.org/abs/2304.01196)

19. [马斯克叫停 GPT-5 研究，意大利禁用 ChatGPT ，生成式 AI 最大风险是什么？该如何监管？](https://www.zhihu.com/question/593135336)

20. [手把手教你注册和使用ChatGPT](https://juejin.cn/post/7199657558834692157)

21. [搞懂GPT，只需看这些！](https://zhuanlan.zhihu.com/p/403469926)
22. [完全图解GPT-2：看完这篇就够了（一）](https://zhuanlan.zhihu.com/p/343922021)
23. [GPT-4 发布后，你的 NLP 研究发生了怎样的变化？](https://zhuanlan.zhihu.com/p/618587452)

24. [人工智能领域常用的开源框架和库（含机器学习/深度学习/强化学习/知识图谱/图神经网络）](https://www.cnblogs.com/zhengzhicong/p/12875348.html)

25. [机器学习、深度学习和强化学习的关系和区别是什么？](https://www.zhihu.com/question/279973545)

26. [DEEP REINFORCEMENT LEARNING](https://arxiv.org/pdf/1810.06339.pdf)

27. [130页 PPT 深入浅出了解 ChatGPT —— ChatGPT 从 0 到 1](https://zhuanlan.zhihu.com/p/616968861)
28. ~~[ChatGPT 从入门到精通 最全教程                      ](https://zhuanlan.zhihu.com/p/635434782)~~

29. ~~[《ChatGPT从入门到精通》-群鸟网](https://zhuanlan.zhihu.com/p/612216936):~~ <https://www.qunniao.cn/tags/1539.html>

30. [对话生成模型总结（解读+开源代码）](https://zhuanlan.zhihu.com/p/53624766)

31. [ChatGPT 教程 - 从入门到精通-part1](https://blog.csdn.net/rucoding/article/details/130693578)
32. [ChatGPT 教程 - 从入门到精通-part2](https://blog.csdn.net/rucoding/article/details/130694108)

33. [ChatGPT学习笔记](https://zhuanlan.zhihu.com/p/619251228)

34. [《Deep Learning》](https://www.zhihu.com/question/37972263)

35. [中国人工智能学会](https://www.caai.cn)
36. [中国人工智能学会数字图书馆](http://dl.caai.cn)

37. [脑机接口](https://xn--dl-0j6cq11d8ge830c.caai.cn/home/view/show/id/240.html)

38. [文心一言](https://yiyan.baidu.com)
39. [文心一格](https://yige.baidu.com)

40. [支持向量机原理       ](https://blog.csdn.net/yuxiaoye03222/article/details/108269311)
41. [SMO算法笔记及个人理解](https://blog.csdn.net/anchor_jun/article/details/122504065)

42. [支持向量机原理解析  ](https://zhuanlan.zhihu.com/p/339929406)
43. [神经网络与支持向量机](https://zhuanlan.zhihu.com/p/29586189)

44. [支持向量机神经网络对比分析](https://www.codenong.com/cs107079623)

45. [Using Analytic QP and Sparseness to Speed Training of Support Vector Machines](https://proceedings.neurips.cc/paper_files/paper/1998/file/7e1d842d0f7ee600116ffc6b2d87d83f-Paper.pdf)

46. [Huggingface简介及BERT代码浅析         ](https://zhuanlan.zhihu.com/p/120315111)
47. [Hugging Face Hub你探索更多AI模型和应用](https://zhuanlan.zhihu.com/p/623521984)

48. [ChatGPT 中文调教指南](https://github.com/PlexPt/awesome-chatgpt-prompts-zh)

49. [ChatGPT学习笔记](https://zhuanlan.zhihu.com/p/619251228)

50. [Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)

51. [神经元BigNeuron脑科学](https://neuromorpho.org), <https://www.nature.com/articles/520013a>, <https://www.nature.com/articles/s41592-023-01848-5>

52. [NiuTensor张量计算库](https://opensource.niutrans.com/niutensor/index.html)

53. [Transformer模型训练技术简介](https://zhuanlan.zhihu.com/p/438150240)

54. <https://tridao.me/publications/flash2/flash2.pdf>

55. [人工智能](https://zhuanlan.zhihu.com/p/26727470)

56. [人工智能PDF中文教材资源](https://zhuanlan.zhihu.com/p/34312502)

57. [scipy中pdist和squareform](https://blog.csdn.net/qq_20135597/article/details/94212816)

58. [numpy的partition和argpartition](https://www.zhihu.com/question/304282758)

59. [Implementing Word2Vec in PyTorch](https://muhark.github.io/python/ml/nlp/2021/10/21/word2vec-from-scratch.html)

60. [使用nltk删除英文停用词](https://zhuanlan.zhihu.com/p/34671514)

61. [NLTK中的Stemmers](https://www.cnblogs.com/patrick-l/p/12251747.html)

62. [Datasets快速使用](https://zhuanlan.zhihu.com/p/548355568)

63. <https://www.nltk.org>

64. <https://tqdm.github.io>

65. [自然语言处理（spacy）](https://zhuanlan.zhihu.com/p/383933287)

66. [BERT可视化工具bertviz体验](https://zhuanlan.zhihu.com/p/457043243), [BertViz](https://www.cnblogs.com/chinasoft/p/17507405.html)

67. [从零开始实现Transformer](https://zhuanlan.zhihu.com/p/651736596)

68. [Huggingface Transformers](https://zhuanlan.zhihu.com/p/448852278)

69. [Transformer 训练与评估](https://zhuanlan.zhihu.com/p/97451231)

70. [交叉熵（cross-entropy）损失函数求导过程推导](https://blog.csdn.net/weixin_43846347/article/details/94363273)
71. [关于损失函数的一些前置知识                 ](https://blog.csdn.net/weixin_42426841/article/details/139886542)
72. [交叉熵损失函数详解和要点提醒               ](https://blog.csdn.net/weixin_42426841/article/details/139889247)

73. <https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot>

74. <https://blog.langchain.dev/retrieval>, <https://cookbook.langchain.com.cn/docs/langchain-intro>

89. [ChatGPT and Competing LLMs                                                                                ](https://www.oreilly.com/live-events/chatgpt-and-competing-llms/0636920097613): <https://github.com/DataForScience/ChatGPT>
90. [ChatGPT for Software Engineers                                                                            ](https://www.oreilly.com/live-events/chatgpt-for-software-engineers/0636920090062)
91. [Prompt Engineering for Generative AI                                                                      ](https://www.oreilly.com/library/view/prompt-engineering-for/9781098153427): <https://github.com/BrightPool/prompt-engineering-for-generative-ai-examples.git>
92. [Language Models in Plain English                                                                          ](https://www.oreilly.com/library/view/language-models-in/9781098109073)
93. [What Are ChatGPT and Its Friends?                                                                         ](https://www.oreilly.com/library/view/what-are-chatgpt/9781098152604)
94. [Quick Start Guide to Large Language Models: Strategies and Best Practices for Using ChatGPT and Other LLMs](https://www.oreilly.com/library/view/quick-start-guide/9780138199425)
95. [Introduction to Transformer Models for NLP                                                                ](https://learning.oreilly.com/course/introduction-to-transformer/9780137923717)
96. [Natural Language Processing, 2nd Edition                                                                  ](https://learning.oreilly.com/course/natural-language-processing/9780137670222)
97. [ChatGPT Shortcuts                                                                                         ](https://learning.oreilly.com/playlists/1a47d633-5de3-4363-9e6e-2ea9ec1a60d5)
98. [How AI Works                                                                                              ](https://learning.oreilly.com/library/view/how-ai-work/9781098168568)
99. [Hacking Artificial Intelligence                                                                           ](https://learning.oreilly.com/videos/hacking-artificial-intelligence/9781663719379)

100. [深度求索](https://www.deepseek.com): <https://api-docs.deepseek.com/zh-cn>
101. [豆包](https://www.doubao.com)

102. <https://www.office.com/?auth=1>

103. <https://developer.microsoft.com>
104. <https://developer.microsoft.com/zh-cn/azure>
105. <https://developer.microsoft.com/en-us/microsoft-365/profile>

106. <https://learn.microsoft.com/>
107. <https://learn.microsoft.com/zh-cn/graph/api/resources/onedrive?view=graph-rest-1.0>

108. <https://www.microsoft365.com/>
109. <https://www.microsoft365.com/apps?auth=1&home=1>

110. <https://account.microsoft.com/?ref=MeControl>

111. <https://portal.azure.com/>
112. <https://azure.microsoft.com/zh-cn/pricing/purchase-options/azure-account?icid=developer&wt.mc_id=developermscom>

113. <https://learn.microsoft.com/en-us/training/modules/explore-azure-openai/1-introduction>
114. <https://learn.microsoft.com/en-us/training/modules/explore-azure-openai/4-how-to-use-azure-openai>
115. <https://learn.microsoft.com/en-us/training/modules/explore-azure-openai/8a-exercise-openai>

116.  <https://learn.microsoft.com/en-us/azure/ai-services/openai/reference>
117. <https://learn.microsoft.com/en-us/azure/ai-services/openai/quickstart>
118. <https://learn.microsoft.com/en-us/azure/ai-services/authentication>
119. <https://learn.microsoft.com/en-us/azure/ai-services/disable-local-auth>

120. <https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app>
121. <https://learn.microsoft.com/en-us/entra/identity-platform/howto-restrict-your-app-to-a-set-of-users>
122. <https://learn.microsoft.com/en-us/entra/identity-platform/scopes-oidc>
123. <https://learn.microsoft.com/en-us/entra/identity-platform/consent-types-developer>
124. <https://learn.microsoft.com/en-us/entra/identity-platform/msal-acquire-cache-tokens>

125. <https://learn.microsoft.com/en-us/graph/api/drive-sharedwithme>
126. <https://learn.microsoft.com/en-us/graph/api/driveitem-get-content>
127. <https://learn.microsoft.com/en-us/graph/permissions-reference>

