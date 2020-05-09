# bugszero-java
# 题目介绍
Trivia 是风靡欧美的一种益智问答游戏。Trivia 原意指“冷知识”，词源来自于拉丁文的“trivium”，意指“三叉路”。

# 游戏的规则很简单：
每次游戏可允许 2-6 名数量不等的玩家参加

游戏提供“摇滚”（Rock）、“体育”（Sports）、“科学”（Science）、“流行”（Pop）四个类别的题目

四类问题均匀分布在一张首尾循环的 12 宫格地图上，每个格子上都有且仅有一个类别的问题供回答

每轮开始系统将为玩家投掷一个 6 面骰子，玩家按骰子点数在地图上前进相应步数，并回答该格子下所显示类别的题目

若骰子点数为奇数，将玩家将从惩罚区（Penalty Box）释放，回到游戏中继续前进、回答问题
若骰子点数为偶数，则惩罚区中的玩家保持位置不变、不能回答问题，直接跳到下一位玩家
每个类别均有 50 个备选问题，玩家回答的问题由系统随机选择

玩家依次轮流回答问题，每道回答正确的问题玩家将得到 1 枚金币

题目回答错误的玩家将被送到惩罚区

首先得到 6 枚金币的玩家即为获胜，游戏结束
我们已经为这个游戏开发了一个系统，系统即将完成，但还存在一些 bug，而且后期还有一些需求变更尚未实现。如果你能帮我们多做一点新特性的开发和缺陷修复，那便真是太好了！

bug：进入惩罚区的玩家不应该再回答问题

bug：金币被奖励给了错误的玩家

bug：题目集有可能用尽

新功能：新增两个类别的问题：蓝调（Blues）、历史（History）

保证问题分布均匀
保证能得到正确类别的题目
请使用下面的命令拉取/构建代码：

Java:
--
git@github.com:chengkunxf/bugszero-java.git

git checkout master

cd java

./gradlew clean build

JavaScript：
--
git clone git@github.com:linesh-simplicity/BugsZero-Kata.git
git checkout master
cd BugsZero-Kata/javascript
npm i
npm test
