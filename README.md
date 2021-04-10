## 相关介绍
这是一个简易的LeetCode自动统计程序, 可自动统计最近提交通过的题目, 并以Markdown的形式展示相关的数据。
根据个人需求, 我只重点获取**提交次数**和**重刷次数**这两个指标, 目的是为了更好地辅助做题。
## 使用教程
1. Fork本仓库
2. 配置GitHub Actions所需的参数
    - 点击仓库下的Settings->Secrets->New repository secret, 分别添加以下secret
        - Name:LEETCODE_EMAIL  Value:你的LeetCode账号
        - Name:LEETCODE_PASSWORD  Value:你的LeetCode密码
    - 点击[tokens](https://github.com/settings/tokens)->Generate new token
        - Note:GITHUB_TOKEN
        - Select scopes:建议全部勾选
    - 修改[action.yml](.github/workflows/action.yml)文件的第`42行`, 将`email`更改为你的GitHub邮箱地址
    - 修改[action.yml](.github/workflows/action.yml)文件的第`43行`, 将`name`更改为你的GitHub用户名
3. 默认配置为12小时更新一次，可根据需求修改[action.yml](.github/workflows/action.yml)文件的第`6行`
## 补充说明
如有其他需求, 欢迎提交PR。


> 重刷次数的计算规则为: 累计所有提交通过且互为不同一天的记录次数

| 最近提交时间 | 题目 | 题目难度 | 提交次数| 重刷次数 |
| ---- | ---- | ---- | ---- | ---- |
| 2021-04-10 08:16 | [#263 丑数](https://leetcode-cn.com/problems/ugly-number) | EASY | 2 | 1 |
| 2021-03-06 07:55 | [#144 二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal) | MEDIUM | 3 | **3** |
| 2021-03-01 11:07 | [#303 区域和检索 - 数组不可变](https://leetcode-cn.com/problems/range-sum-query-immutable) | EASY | 3 | 1 |
| 2021-03-01 10:55 | [#896 单调数列](https://leetcode-cn.com/problems/monotonic-array) | EASY | 2 | 1 |
| 2021-02-25 14:50 | [#867 转置矩阵](https://leetcode-cn.com/problems/transpose-matrix) | EASY | 1 | 1 |
| 2021-02-23 14:54 | [#1052 爱生气的书店老板](https://leetcode-cn.com/problems/grumpy-bookstore-owner) | MEDIUM | 1 | 1 |
| 2021-02-22 13:14 | [#766 托普利茨矩阵](https://leetcode-cn.com/problems/toeplitz-matrix) | EASY | 2 | 1 |
| 2021-02-21 11:52 | [#1438 绝对差不超过限制的最长连续子数组](https://leetcode-cn.com/problems/longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit) | MEDIUM | 2 | 1 |
| 2021-02-20 16:09 | [#1763 最长的美好子字符串](https://leetcode-cn.com/problems/longest-nice-substring) | EASY | 5 | 1 |
| 2021-02-20 13:30 | [#1759 统计同构子字符串的数目](https://leetcode-cn.com/problems/count-number-of-homogenous-substrings) | MEDIUM | 10 | 1 |
| 2021-02-20 02:59 | [#697 数组的度](https://leetcode-cn.com/problems/degree-of-an-array) | EASY | 1 | 1 |
| 2021-02-19 16:47 | [#435 无重叠区间](https://leetcode-cn.com/problems/non-overlapping-intervals) | MEDIUM | 4 | 1 |
| 2021-02-19 15:30 | [#41 缺失的第一个正数](https://leetcode-cn.com/problems/first-missing-positive) | HARD | 6 | **2** |
| 2021-02-19 14:41 | [#617 合并二叉树](https://leetcode-cn.com/problems/merge-two-binary-trees) | EASY | 2 | 1 |
| 2021-02-19 14:18 | [#9 回文数](https://leetcode-cn.com/problems/palindrome-number) | EASY | 2 | 1 |
| 2021-02-19 14:01 | [#1004 最大连续1的个数 III](https://leetcode-cn.com/problems/max-consecutive-ones-iii) | MEDIUM | 6 | 1 |
| 2021-02-18 14:08 | [#925 长按键入](https://leetcode-cn.com/problems/long-pressed-name) | EASY | 5 | 1 |
| 2021-02-18 13:42 | [#455 分发饼干](https://leetcode-cn.com/problems/assign-cookies) | EASY | 4 | **3** |
| 2021-02-18 13:28 | [#995 K 连续位的最小翻转次数](https://leetcode-cn.com/problems/minimum-number-of-k-consecutive-bit-flips) | HARD | 1 | 1 |
| 2021-02-17 09:44 | [#61 旋转链表](https://leetcode-cn.com/problems/rotate-list) | MEDIUM | 3 | 1 |
| 2021-02-17 09:20 | [#86 分隔链表](https://leetcode-cn.com/problems/partition-list) | MEDIUM | 1 | 1 |
| 2021-02-17 07:57 | [#7 整数反转](https://leetcode-cn.com/problems/reverse-integer) | EASY | 6 | 1 |
| 2021-02-17 06:26 | [#566 重塑矩阵](https://leetcode-cn.com/problems/reshape-the-matrix) | EASY | 1 | 1 |
| 2021-02-16 15:21 | [#575 分糖果](https://leetcode-cn.com/problems/distribute-candies) | EASY | 2 | 1 |
| 2021-02-16 15:09 | [#561 数组拆分 I](https://leetcode-cn.com/problems/array-partition-i) | EASY | 1 | 1 |
| 2021-02-16 15:00 | [#524 通过删除字母匹配到字典里最长单词](https://leetcode-cn.com/problems/longest-word-in-dictionary-through-deleting) | MEDIUM | 5 | 1 |
| 2021-02-15 16:06 | [#141 环形链表](https://leetcode-cn.com/problems/linked-list-cycle) | EASY | 2 | **2** |
| 2021-02-15 15:58 | [#88 合并两个有序数组](https://leetcode-cn.com/problems/merge-sorted-array) | EASY | 4 | **2** |
| 2021-02-15 14:25 | [#345 反转字符串中的元音字母](https://leetcode-cn.com/problems/reverse-vowels-of-a-string) | EASY | 3 | 1 |
| 2021-02-15 14:02 | [#167 两数之和 II - 输入有序数组](https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted) | EASY | 1 | 1 |
| 2021-02-15 12:43 | [#1 两数之和](https://leetcode-cn.com/problems/two-sum) | EASY | 7 | **3** |
| 2021-02-15 09:50 | [#633 平方数之和](https://leetcode-cn.com/problems/sum-of-square-numbers) | MEDIUM | 1 | 1 |
| 2021-02-15 09:39 | [#680 验证回文字符串 Ⅱ](https://leetcode-cn.com/problems/valid-palindrome-ii) | EASY | 1 | 1 |
| 2021-02-15 09:26 | [#485 最大连续 1 的个数](https://leetcode-cn.com/problems/max-consecutive-ones) | EASY | 5 | **2** |
| 2021-02-13 15:17 | [#209 长度最小的子数组](https://leetcode-cn.com/problems/minimum-size-subarray-sum) | MEDIUM | 1 | 1 |
| 2021-02-13 15:07 | [#567 字符串的排列](https://leetcode-cn.com/problems/permutation-in-string) | MEDIUM | 1 | 1 |
| 2021-02-13 11:58 | [#448 找到所有数组中消失的数字](https://leetcode-cn.com/problems/find-all-numbers-disappeared-in-an-array) | EASY | 4 | **3** |
| 2021-02-12 10:01 | [#76 最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring) | HARD | 5 | **2** |
| 2021-02-12 09:29 | [#703 数据流中的第 K 大元素](https://leetcode-cn.com/problems/kth-largest-element-in-a-stream) | EASY | 3 | **2** |
| 2021-02-12 08:53 | [#119 杨辉三角 II](https://leetcode-cn.com/problems/pascals-triangle-ii) | EASY | 4 | 1 |
| 2021-02-10 03:20 | [#424 替换后的最长重复字符](https://leetcode-cn.com/problems/longest-repeating-character-replacement) | MEDIUM | 1 | 1 |
| 2021-02-09 06:50 | [#992 K 个不同整数的子数组](https://leetcode-cn.com/problems/subarrays-with-k-different-integers) | HARD | 3 | 1 |
| 2021-02-08 09:20 | [#978 最长湍流子数组](https://leetcode-cn.com/problems/longest-turbulent-subarray) | MEDIUM | 1 | 1 |
| 2021-02-07 09:24 | [#6 Z 字形变换](https://leetcode-cn.com/problems/zigzag-conversion) | MEDIUM | 2 | 1 |
| 2021-02-07 07:18 | [#665 非递减数列](https://leetcode-cn.com/problems/non-decreasing-array) | EASY | 3 | 1 |
| 2021-01-31 14:49 | [#面试题 01.04 回文排列](https://leetcode-cn.com/problems/palindrome-permutation-lcci) | EASY | 1 | 1 |
| 2021-01-30 10:06 | [#面试题 01.03 URL化](https://leetcode-cn.com/problems/string-to-url-lcci) | EASY | 3 | 1 |
| 2021-01-30 08:05 | [#面试题 01.02 判定是否互为字符重排](https://leetcode-cn.com/problems/check-permutation-lcci) | EASY | 1 | 1 |
| 2021-01-30 08:00 | [#面试题 01.01 判定字符是否唯一](https://leetcode-cn.com/problems/is-unique-lcci) | EASY | 3 | **3** |
| 2021-01-26 16:42 | [#1128 等价多米诺骨牌对的数量](https://leetcode-cn.com/problems/number-of-equivalent-domino-pairs) | EASY | 1 | 1 |
| 2021-01-20 15:36 | [#628 三个数的最大乘积](https://leetcode-cn.com/problems/maximum-product-of-three-numbers) | EASY | 3 | 1 |
| 2021-01-20 14:19 | [#56 合并区间](https://leetcode-cn.com/problems/merge-intervals) | MEDIUM | 2 | 1 |
| 2021-01-08 05:00 | [#116 填充每个节点的下一个右侧节点指针](https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node) | MEDIUM | 4 | **2** |
| 2021-01-08 04:34 | [#226 翻转二叉树](https://leetcode-cn.com/problems/invert-binary-tree) | EASY | 3 | **3** |
| 2021-01-07 10:23 | [#113 路径总和 II](https://leetcode-cn.com/problems/path-sum-ii) | MEDIUM | 3 | 1 |
| 2021-01-07 08:51 | [#112 路径总和](https://leetcode-cn.com/problems/path-sum) | EASY | 3 | 1 |
| 2021-01-07 01:38 | [#92 反转链表 II](https://leetcode-cn.com/problems/reverse-linked-list-ii) | MEDIUM | 6 | **3** |
| 2021-01-05 15:09 | [#剑指 Offer 24 反转链表](https://leetcode-cn.com/problems/fan-zhuan-lian-biao-lcof) | EASY | 8 | **3** |
| 2021-01-05 14:06 | [#1046 最后一块石头的重量](https://leetcode-cn.com/problems/last-stone-weight) | EASY | 2 | **2** |
| 2020-12-25 06:49 | [#42 接雨水](https://leetcode-cn.com/problems/trapping-rain-water) | HARD | 7 | **3** |
| 2020-12-24 15:07 | [#135 分发糖果](https://leetcode-cn.com/problems/candy) | HARD | 8 | 1 |
| 2020-12-21 15:43 | [#316 去除重复字母](https://leetcode-cn.com/problems/remove-duplicate-letters) | MEDIUM | 6 | 1 |
| 2020-12-20 06:59 | [#49 字母异位词分组](https://leetcode-cn.com/problems/group-anagrams) | MEDIUM | 3 | 1 |
| 2020-12-20 03:03 | [#861 翻转矩阵后的得分](https://leetcode-cn.com/problems/score-after-flipping-matrix) | MEDIUM | 2 | 1 |
| 2020-10-28 04:53 | [#20 有效的括号](https://leetcode-cn.com/problems/valid-parentheses) | EASY | 7 | **3** |
| 2020-10-18 15:30 | [#55 跳跃游戏](https://leetcode-cn.com/problems/jump-game) | MEDIUM | 4 | 1 |
| 2020-10-18 04:47 | [#401 二进制手表](https://leetcode-cn.com/problems/binary-watch) | EASY | 3 | 1 |
| 2020-10-15 07:01 | [#145 二叉树的后序遍历](https://leetcode-cn.com/problems/binary-tree-postorder-traversal) | MEDIUM | 3 | **3** |
| 2020-10-15 06:34 | [#94 二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal) | MEDIUM | 2 | **2** |
| 2020-10-14 16:18 | [#402 移掉K位数字](https://leetcode-cn.com/problems/remove-k-digits) | MEDIUM | 3 | 1 |
| 2020-10-14 14:37 | [#376 摆动序列](https://leetcode-cn.com/problems/wiggle-subsequence) | MEDIUM | 4 | 1 |
| 2020-10-09 13:59 | [#344 反转字符串](https://leetcode-cn.com/problems/reverse-string) | EASY | 1 | 1 |
| 2020-10-07 12:48 | [#84 柱状图中最大的矩形](https://leetcode-cn.com/problems/largest-rectangle-in-histogram) | HARD | 1 | 1 |
| 2020-10-07 12:08 | [#75 颜色分类](https://leetcode-cn.com/problems/sort-colors) | MEDIUM | 1 | 1 |
| 2020-10-02 13:03 | [#771 宝石与石头](https://leetcode-cn.com/problems/jewels-and-stones) | EASY | 1 | 1 |
| 2020-10-02 12:56 | [#LCP 19 秋叶收藏集](https://leetcode-cn.com/problems/UlBDOe) | MEDIUM | 2 | 1 |
| 2020-10-02 11:27 | [#117 填充每个节点的下一个右侧节点指针 II](https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node-ii) | MEDIUM | 3 | **2** |
| 2020-09-30 13:58 | [#701 二叉搜索树中的插入操作](https://leetcode-cn.com/problems/insert-into-a-binary-search-tree) | MEDIUM | 2 | 1 |
| 2020-09-29 00:52 | [#108 将有序数组转换为二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-array-to-binary-search-tree) | EASY | 1 | 1 |
| 2020-09-19 09:19 | [#11 盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water) | MEDIUM | 2 | 1 |
| 2020-09-19 07:58 | [#1114 按序打印](https://leetcode-cn.com/problems/print-in-order) | EASY | 2 | 1 |
| 2020-09-19 07:03 | [#剑指 Offer 27 二叉树的镜像](https://leetcode-cn.com/problems/er-cha-shu-de-jing-xiang-lcof) | EASY | 3 | **2** |
| 2020-09-15 00:41 | [#637 二叉树的层平均值](https://leetcode-cn.com/problems/average-of-levels-in-binary-tree) | EASY | 1 | 1 |
| 2020-09-11 09:14 | [#155 最小栈](https://leetcode-cn.com/problems/min-stack) | EASY | 2 | 1 |
| 2020-09-11 02:42 | [#216 组合总和 III](https://leetcode-cn.com/problems/combination-sum-iii) | MEDIUM | 3 | 1 |
| 2020-09-10 07:18 | [#27 移除元素](https://leetcode-cn.com/problems/remove-element) | EASY | 2 | **2** |
| 2020-09-10 06:46 | [#47 全排列 II](https://leetcode-cn.com/problems/permutations-ii) | MEDIUM | 3 | **2** |
| 2020-09-10 06:35 | [#40 组合总和 II](https://leetcode-cn.com/problems/combination-sum-ii) | MEDIUM | 2 | **2** |
| 2020-09-09 08:13 | [#236 二叉树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree) | MEDIUM | 3 | 1 |
| 2020-09-09 03:01 | [#39 组合总和](https://leetcode-cn.com/problems/combination-sum) | MEDIUM | 3 | **2** |
| 2020-09-08 08:51 | [#461 汉明距离](https://leetcode-cn.com/problems/hamming-distance) | EASY | 1 | 1 |
| 2020-09-08 07:45 | [#51 N 皇后](https://leetcode-cn.com/problems/n-queens) | HARD | 1 | 1 |
| 2020-09-08 02:34 | [#77 组合](https://leetcode-cn.com/problems/combinations) | MEDIUM | 9 | 1 |
| 2020-09-07 02:30 | [#347 前 K 个高频元素](https://leetcode-cn.com/problems/top-k-frequent-elements) | MEDIUM | 2 | **2** |
| 2020-09-06 13:27 | [#200 岛屿数量](https://leetcode-cn.com/problems/number-of-islands) | MEDIUM | 1 | 1 |
| 2020-09-06 13:10 | [#136 只出现一次的数字](https://leetcode-cn.com/problems/single-number) | EASY | 1 | 1 |
| 2020-09-06 12:46 | [#107 二叉树的层序遍历 II](https://leetcode-cn.com/problems/binary-tree-level-order-traversal-ii) | MEDIUM | 4 | 1 |
| 2020-09-05 09:31 | [#257 二叉树的所有路径](https://leetcode-cn.com/problems/binary-tree-paths) | EASY | 2 | 1 |
| 2020-09-05 09:07 | [#60 排列序列](https://leetcode-cn.com/problems/permutation-sequence) | HARD | 2 | 1 |
| 2020-09-04 14:38 | [#221 最大正方形](https://leetcode-cn.com/problems/maximal-square) | MEDIUM | 5 | 1 |
| 2020-09-03 10:42 | [#543 二叉树的直径](https://leetcode-cn.com/problems/diameter-of-binary-tree) | EASY | 2 | 1 |
| 2020-09-03 08:49 | [#463 岛屿的周长](https://leetcode-cn.com/problems/island-perimeter) | EASY | 1 | 1 |
| 2020-08-26 03:18 | [#17 电话号码的字母组合](https://leetcode-cn.com/problems/letter-combinations-of-a-phone-number) | MEDIUM | 1 | 1 |
| 2020-08-25 09:18 | [#139 单词拆分](https://leetcode-cn.com/problems/word-break) | MEDIUM | 5 | 1 |
| 2020-08-25 02:31 | [#491 递增子序列](https://leetcode-cn.com/problems/increasing-subsequences) | MEDIUM | 1 | 1 |
| 2020-08-25 00:28 | [#459 重复的子字符串](https://leetcode-cn.com/problems/repeated-substring-pattern) | EASY | 1 | 1 |
| 2020-08-23 13:50 | [#201 数字范围按位与](https://leetcode-cn.com/problems/bitwise-and-of-numbers-range) | MEDIUM | 1 | 1 |
| 2020-08-23 05:50 | [#188 买卖股票的最佳时机 IV](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iv) | HARD | 4 | **2** |
| 2020-08-22 09:15 | [#64 最小路径和](https://leetcode-cn.com/problems/minimum-path-sum) | MEDIUM | 1 | 1 |
| 2020-08-22 08:53 | [#32 最长有效括号](https://leetcode-cn.com/problems/longest-valid-parentheses) | HARD | 5 | 1 |
| 2020-08-21 14:27 | [#111 二叉树的最小深度](https://leetcode-cn.com/problems/minimum-depth-of-binary-tree) | EASY | 6 | 1 |
| 2020-08-21 00:23 | [#178 分数排名](https://leetcode-cn.com/problems/rank-scores) | MEDIUM | 2 | **2** |
| 2020-08-20 13:54 | [#184 部门工资最高的员工](https://leetcode-cn.com/problems/department-highest-salary) | MEDIUM | 4 | 1 |
| 2020-08-20 13:27 | [#183 从不订购的客户](https://leetcode-cn.com/problems/customers-who-never-order) | EASY | 2 | 1 |
| 2020-08-20 13:23 | [#182 查找重复的电子邮箱](https://leetcode-cn.com/problems/duplicate-emails) | EASY | 2 | 1 |
| 2020-08-20 13:02 | [#181 超过经理收入的员工](https://leetcode-cn.com/problems/employees-earning-more-than-their-managers) | EASY | 1 | 1 |
| 2020-08-20 12:33 | [#529 扫雷游戏](https://leetcode-cn.com/problems/minesweeper) | MEDIUM | 2 | 1 |
| 2020-08-20 08:15 | [#177 第N高的薪水](https://leetcode-cn.com/problems/nth-highest-salary) | MEDIUM | 3 | **2** |
| 2020-08-20 08:04 | [#176 第二高的薪水](https://leetcode-cn.com/problems/second-highest-salary) | EASY | 6 | **2** |
| 2020-08-20 07:52 | [#175 组合两个表](https://leetcode-cn.com/problems/combine-two-tables) | EASY | 2 | **2** |
| 2020-08-19 07:20 | [#416 分割等和子集](https://leetcode-cn.com/problems/partition-equal-subset-sum) | MEDIUM | 6 | **2** |
| 2020-08-19 06:47 | [#5 最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring) | MEDIUM | 10 | **3** |
| 2020-08-19 04:27 | [#647 回文子串](https://leetcode-cn.com/problems/palindromic-substrings) | MEDIUM | 4 | **2** |
| 2020-08-18 05:32 | [#109 有序链表转换二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-list-to-binary-search-tree) | MEDIUM | 1 | 1 |
| 2020-08-17 07:53 | [#15 三数之和](https://leetcode-cn.com/problems/3sum) | MEDIUM | 3 | 1 |
| 2020-08-17 05:22 | [#110 平衡二叉树](https://leetcode-cn.com/problems/balanced-binary-tree) | EASY | 2 | 1 |
| 2020-08-16 15:18 | [#733 图像渲染](https://leetcode-cn.com/problems/flood-fill) | EASY | 1 | 1 |
| 2020-08-15 03:42 | [#90 子集 II](https://leetcode-cn.com/problems/subsets-ii) | MEDIUM | 3 | **2** |
| 2020-08-15 03:34 | [#78 子集](https://leetcode-cn.com/problems/subsets) | MEDIUM | 5 | **3** |
| 2020-08-15 01:58 | [#70 爬楼梯](https://leetcode-cn.com/problems/climbing-stairs) | EASY | 2 | 1 |
| 2020-08-13 11:58 | [#46 全排列](https://leetcode-cn.com/problems/permutations) | MEDIUM | 2 | 1 |
| 2020-08-13 10:18 | [#3 无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters) | MEDIUM | 4 | **2** |
| 2020-08-13 10:00 | [#80 删除有序数组中的重复项 II](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array-ii) | MEDIUM | 3 | **2** |
| 2020-08-13 07:55 | [#43 字符串相乘](https://leetcode-cn.com/problems/multiply-strings) | MEDIUM | 3 | 1 |
| 2020-08-13 06:40 | [#53 最大子序和](https://leetcode-cn.com/problems/maximum-subarray) | EASY | 4 | **2** |
| 2020-08-13 04:31 | [#26 删除有序数组中的重复项](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array) | EASY | 2 | **2** |
| 2020-08-13 04:12 | [#2 两数相加](https://leetcode-cn.com/problems/add-two-numbers) | MEDIUM | 4 | **2** |
| 2020-08-12 04:28 | [#133 克隆图](https://leetcode-cn.com/problems/clone-graph) | MEDIUM | 3 | 1 |
| 2020-08-11 12:28 | [#130 被围绕的区域](https://leetcode-cn.com/problems/surrounded-regions) | MEDIUM | 1 | 1 |
| 2020-08-10 02:23 | [#696 计数二进制子串](https://leetcode-cn.com/problems/count-binary-substrings) | EASY | 1 | 1 |
| 2020-08-09 14:49 | [#83 删除排序链表中的重复元素](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list) | EASY | 2 | 1 |
| 2020-08-09 13:05 | [#剑指 Offer 46 把数字翻译成字符串](https://leetcode-cn.com/problems/ba-shu-zi-fan-yi-cheng-zi-fu-chuan-lcof) | MEDIUM | 5 | 1 |
| 2020-08-09 12:17 | [#93 复原 IP 地址](https://leetcode-cn.com/problems/restore-ip-addresses) | MEDIUM | 3 | 1 |
| 2020-08-09 03:26 | [#1545 找出第 N 个二进制字符串中的第 K 位](https://leetcode-cn.com/problems/find-kth-bit-in-nth-binary-string) | MEDIUM | 3 | 1 |
| 2020-08-09 03:04 | [#1544 整理字符串](https://leetcode-cn.com/problems/make-the-string-great) | EASY | 1 | 1 |
| 2020-08-08 01:21 | [#123 买卖股票的最佳时机 III](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iii) | HARD | 3 | **2** |
| 2020-08-07 14:03 | [#309 最佳买卖股票时机含冷冻期](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown) | MEDIUM | 2 | 1 |
| 2020-08-07 13:38 | [#714 买卖股票的最佳时机含手续费](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee) | MEDIUM | 2 | 1 |
| 2020-08-07 08:57 | [#100 相同的树](https://leetcode-cn.com/problems/same-tree) | EASY | 2 | 1 |
| 2020-08-07 08:29 | [#122 买卖股票的最佳时机 II](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii) | EASY | 2 | 1 |
| 2020-08-06 15:40 | [#121 买卖股票的最佳时机](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock) | EASY | 1 | 1 |
| 2020-08-05 05:05 | [#494 目标和](https://leetcode-cn.com/problems/target-sum) | MEDIUM | 2 | 1 |
| 2020-08-05 03:04 | [#234 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list) | EASY | 1 | 1 |
| 2020-08-05 02:04 | [#337 打家劫舍 III](https://leetcode-cn.com/problems/house-robber-iii) | MEDIUM | 2 | **2** |
| 2020-08-04 14:54 | [#207 课程表](https://leetcode-cn.com/problems/course-schedule) | MEDIUM | 2 | 1 |
| 2020-08-04 02:03 | [#146 LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache) | MEDIUM | 1 | 1 |
| 2020-08-03 08:36 | [#338 比特位计数](https://leetcode-cn.com/problems/counting-bits) | MEDIUM | 3 | 1 |
| 2020-08-03 05:23 | [#213 打家劫舍 II](https://leetcode-cn.com/problems/house-robber-ii) | MEDIUM | 5 | 1 |
| 2020-08-03 04:49 | [#198 打家劫舍](https://leetcode-cn.com/problems/house-robber) | MEDIUM | 4 | 1 |
| 2020-08-03 03:23 | [#415 字符串相加](https://leetcode-cn.com/problems/add-strings) | EASY | 2 | 1 |
| 2020-08-02 07:07 | [#206 反转链表](https://leetcode-cn.com/problems/reverse-linked-list) | EASY | 2 | 1 |
| 2020-08-02 03:59 | [#96 不同的二叉搜索树](https://leetcode-cn.com/problems/unique-binary-search-trees) | MEDIUM | 1 | 1 |
| 2020-08-02 01:50 | [#114 二叉树展开为链表](https://leetcode-cn.com/problems/flatten-binary-tree-to-linked-list) | MEDIUM | 1 | 1 |
| 2020-08-01 12:28 | [#98 验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree) | MEDIUM | 2 | 1 |
| 2020-08-01 02:00 | [#面试题 08.03 魔术索引](https://leetcode-cn.com/problems/magic-index-lcci) | EASY | 2 | 1 |
| 2020-08-01 01:08 | [#101 对称二叉树](https://leetcode-cn.com/problems/symmetric-tree) | EASY | 2 | 1 |
| 2020-07-30 07:09 | [#104 二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree) | EASY | 1 | 1 |
| 2020-07-30 07:01 | [#343 整数拆分](https://leetcode-cn.com/problems/integer-break) | MEDIUM | 1 | 1 |
| 2020-07-30 06:46 | [#62 不同路径](https://leetcode-cn.com/problems/unique-paths) | MEDIUM | 2 | 1 |
| 2020-07-30 02:33 | [#79 单词搜索](https://leetcode-cn.com/problems/word-search) | MEDIUM | 4 | 1 |
| 2020-07-28 03:17 | [#38 外观数列](https://leetcode-cn.com/problems/count-and-say) | EASY | 1 | 1 |
| 2020-07-28 02:30 | [#剑指 Offer 45 把数组排成最小的数](https://leetcode-cn.com/problems/ba-shu-zu-pai-cheng-zui-xiao-de-shu-lcof) | MEDIUM | 1 | 1 |
| 2020-07-27 09:23 | [#剑指 Offer 33 二叉搜索树的后序遍历序列](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-de-hou-xu-bian-li-xu-lie-lcof) | MEDIUM | 2 | 1 |
| 2020-07-27 05:40 | [#剑指 Offer 47 礼物的最大价值](https://leetcode-cn.com/problems/li-wu-de-zui-da-jie-zhi-lcof) | MEDIUM | 3 | 1 |
| 2020-07-27 02:14 | [#剑指 Offer 48 最长不含重复字符的子字符串](https://leetcode-cn.com/problems/zui-chang-bu-han-zhong-fu-zi-fu-de-zi-zi-fu-chuan-lcof) | MEDIUM | 4 | 1 |
| 2020-07-26 03:47 | [#剑指 Offer 20 表示数值的字符串](https://leetcode-cn.com/problems/biao-shi-shu-zhi-de-zi-fu-chuan-lcof) | MEDIUM | 7 | 1 |
| 2020-07-24 05:49 | [#剑指 Offer 14- II 剪绳子 II](https://leetcode-cn.com/problems/jian-sheng-zi-ii-lcof) | MEDIUM | 1 | 1 |
| 2020-07-24 05:38 | [#剑指 Offer 14- I 剪绳子](https://leetcode-cn.com/problems/jian-sheng-zi-lcof) | MEDIUM | 1 | 1 |
| 2020-07-23 08:17 | [#剑指 Offer 63 股票的最大利润](https://leetcode-cn.com/problems/gu-piao-de-zui-da-li-run-lcof) | MEDIUM | 1 | 1 |
| 2020-07-23 06:26 | [#剑指 Offer 67 把字符串转换成整数](https://leetcode-cn.com/problems/ba-zi-fu-chuan-zhuan-huan-cheng-zheng-shu-lcof) | MEDIUM | 5 | 1 |
| 2020-07-23 02:59 | [#剑指 Offer 66 构建乘积数组](https://leetcode-cn.com/problems/gou-jian-cheng-ji-shu-zu-lcof) | MEDIUM | 1 | 1 |
| 2020-07-23 01:28 | [#剑指 Offer 64 求1+2+…+n](https://leetcode-cn.com/problems/qiu-12n-lcof) | MEDIUM | 2 | 1 |
| 2020-07-22 03:20 | [#剑指 Offer 61 扑克牌中的顺子](https://leetcode-cn.com/problems/bu-ke-pai-zhong-de-shun-zi-lcof) | EASY | 1 | 1 |
| 2020-07-22 03:01 | [#剑指 Offer 59 - II 队列的最大值](https://leetcode-cn.com/problems/dui-lie-de-zui-da-zhi-lcof) | MEDIUM | 1 | 1 |
| 2020-07-22 01:54 | [#239 滑动窗口最大值](https://leetcode-cn.com/problems/sliding-window-maximum) | HARD | 1 | 1 |
| 2020-07-22 01:51 | [#剑指 Offer 59 - I 滑动窗口的最大值](https://leetcode-cn.com/problems/hua-dong-chuang-kou-de-zui-da-zhi-lcof) | HARD | 1 | 1 |
| 2020-07-21 04:25 | [#剑指 Offer 58 - II 左旋转字符串](https://leetcode-cn.com/problems/zuo-xuan-zhuan-zi-fu-chuan-lcof) | EASY | 1 | 1 |
| 2020-07-21 03:41 | [#剑指 Offer 58 - I 翻转单词顺序](https://leetcode-cn.com/problems/fan-zhuan-dan-ci-shun-xu-lcof) | EASY | 1 | 1 |
| 2020-07-21 03:01 | [#剑指 Offer 57 - II 和为s的连续正数序列](https://leetcode-cn.com/problems/he-wei-sde-lian-xu-zheng-shu-xu-lie-lcof) | EASY | 1 | 1 |
| 2020-07-21 02:13 | [#剑指 Offer 57 和为s的两个数字](https://leetcode-cn.com/problems/he-wei-sde-liang-ge-shu-zi-lcof) | EASY | 1 | 1 |
| 2020-07-21 01:48 | [#剑指 Offer 56 - II 数组中数字出现的次数 II](https://leetcode-cn.com/problems/shu-zu-zhong-shu-zi-chu-xian-de-ci-shu-ii-lcof) | MEDIUM | 2 | 1 |
| 2020-07-21 01:04 | [#剑指 Offer 56 - I 数组中数字出现的次数](https://leetcode-cn.com/problems/shu-zu-zhong-shu-zi-chu-xian-de-ci-shu-lcof) | MEDIUM | 2 | 1 |
| 2020-07-20 09:05 | [#剑指 Offer 55 - II 平衡二叉树](https://leetcode-cn.com/problems/ping-heng-er-cha-shu-lcof) | EASY | 1 | 1 |
| 2020-07-20 08:31 | [#剑指 Offer 55 - I 二叉树的深度](https://leetcode-cn.com/problems/er-cha-shu-de-shen-du-lcof) | EASY | 2 | 1 |
| 2020-07-20 08:06 | [#剑指 Offer 54 二叉搜索树的第k大节点](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-de-di-kda-jie-dian-lcof) | EASY | 1 | 1 |
| 2020-07-20 07:19 | [#剑指 Offer 53 - II 0～n-1中缺失的数字](https://leetcode-cn.com/problems/que-shi-de-shu-zi-lcof) | EASY | 1 | 1 |
| 2020-07-20 06:04 | [#剑指 Offer 53 - I 在排序数组中查找数字 I](https://leetcode-cn.com/problems/zai-pai-xu-shu-zu-zhong-cha-zhao-shu-zi-lcof) | EASY | 2 | 1 |
| 2020-07-12 13:12 | [#剑指 Offer 52 两个链表的第一个公共节点](https://leetcode-cn.com/problems/liang-ge-lian-biao-de-di-yi-ge-gong-gong-jie-dian-lcof) | EASY | 1 | 1 |
| 2020-07-12 03:38 | [#剑指 Offer 50 第一个只出现一次的字符](https://leetcode-cn.com/problems/di-yi-ge-zhi-chu-xian-yi-ci-de-zi-fu-lcof) | EASY | 2 | 1 |
| 2020-07-11 08:10 | [#剑指 Offer 42 连续子数组的最大和](https://leetcode-cn.com/problems/lian-xu-zi-shu-zu-de-zui-da-he-lcof) | EASY | 1 | 1 |
| 2020-07-11 02:38 | [#322 零钱兑换](https://leetcode-cn.com/problems/coin-change) | MEDIUM | 1 | 1 |
| 2020-07-11 02:15 | [#509 斐波那契数](https://leetcode-cn.com/problems/fibonacci-number) | EASY | 8 | 1 |
| 2020-07-10 09:13 | [#剑指 Offer 40 最小的k个数](https://leetcode-cn.com/problems/zui-xiao-de-kge-shu-lcof) | EASY | 6 | 1 |
| 2020-07-10 03:26 | [#剑指 Offer 39 数组中出现次数超过一半的数字](https://leetcode-cn.com/problems/shu-zu-zhong-chu-xian-ci-shu-chao-guo-yi-ban-de-shu-zi-lcof) | EASY | 3 | 1 |
| 2020-07-10 02:06 | [#剑指 Offer 38 字符串的排列](https://leetcode-cn.com/problems/zi-fu-chuan-de-pai-lie-lcof) | MEDIUM | 1 | 1 |
| 2020-07-10 00:53 | [#剑指 Offer 36 二叉搜索树与双向链表](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-yu-shuang-xiang-lian-biao-lcof) | MEDIUM | 2 | 1 |
| 2020-07-09 05:11 | [#剑指 Offer 35 复杂链表的复制](https://leetcode-cn.com/problems/fu-za-lian-biao-de-fu-zhi-lcof) | MEDIUM | 3 | 1 |
| 2020-07-09 02:10 | [#剑指 Offer 34 二叉树中和为某一值的路径](https://leetcode-cn.com/problems/er-cha-shu-zhong-he-wei-mou-yi-zhi-de-lu-jing-lcof) | MEDIUM | 3 | 1 |
| 2020-07-07 06:10 | [#剑指 Offer 32 - III 从上到下打印二叉树 III](https://leetcode-cn.com/problems/cong-shang-dao-xia-da-yin-er-cha-shu-iii-lcof) | MEDIUM | 4 | 1 |
| 2020-07-06 16:46 | [#剑指 Offer 32 - II 从上到下打印二叉树 II](https://leetcode-cn.com/problems/cong-shang-dao-xia-da-yin-er-cha-shu-ii-lcof) | EASY | 1 | 1 |
| 2020-07-06 14:26 | [#剑指 Offer 32 - I 从上到下打印二叉树](https://leetcode-cn.com/problems/cong-shang-dao-xia-da-yin-er-cha-shu-lcof) | MEDIUM | 1 | 1 |
| 2020-07-05 07:31 | [#剑指 Offer 31 栈的压入、弹出序列](https://leetcode-cn.com/problems/zhan-de-ya-ru-dan-chu-xu-lie-lcof) | MEDIUM | 3 | 1 |
| 2020-07-05 05:21 | [#剑指 Offer 30 包含min函数的栈](https://leetcode-cn.com/problems/bao-han-minhan-shu-de-zhan-lcof) | EASY | 4 | 1 |
| 2020-07-03 10:08 | [#剑指 Offer 29 顺时针打印矩阵](https://leetcode-cn.com/problems/shun-shi-zhen-da-yin-ju-zhen-lcof) | EASY | 2 | 1 |
| 2020-07-03 07:33 | [#剑指 Offer 28 对称的二叉树](https://leetcode-cn.com/problems/dui-cheng-de-er-cha-shu-lcof) | EASY | 2 | 1 |
| 2020-07-03 05:05 | [#剑指 Offer 25 合并两个排序的链表](https://leetcode-cn.com/problems/he-bing-liang-ge-pai-xu-de-lian-biao-lcof) | EASY | 1 | 1 |
| 2020-07-03 03:31 | [#剑指 Offer 22 链表中倒数第k个节点](https://leetcode-cn.com/problems/lian-biao-zhong-dao-shu-di-kge-jie-dian-lcof) | EASY | 2 | **2** |
| 2020-07-02 14:16 | [#剑指 Offer 21 调整数组顺序使奇数位于偶数前面](https://leetcode-cn.com/problems/diao-zheng-shu-zu-shun-xu-shi-qi-shu-wei-yu-ou-shu-qian-mian-lcof) | EASY | 2 | 1 |
| 2020-07-02 13:43 | [#剑指 Offer 18 删除链表的节点](https://leetcode-cn.com/problems/shan-chu-lian-biao-de-jie-dian-lcof) | EASY | 1 | 1 |
| 2020-07-02 13:32 | [#剑指 Offer 17 打印从1到最大的n位数](https://leetcode-cn.com/problems/da-yin-cong-1dao-zui-da-de-nwei-shu-lcof) | EASY | 1 | 1 |
| 2020-07-02 10:11 | [#剑指 Offer 16 数值的整数次方](https://leetcode-cn.com/problems/shu-zhi-de-zheng-shu-ci-fang-lcof) | MEDIUM | 2 | 1 |
| 2020-07-02 09:19 | [#剑指 Offer 15 二进制中1的个数](https://leetcode-cn.com/problems/er-jin-zhi-zhong-1de-ge-shu-lcof) | EASY | 2 | 1 |
| 2020-06-29 09:21 | [#剑指 Offer 13 机器人的运动范围](https://leetcode-cn.com/problems/ji-qi-ren-de-yun-dong-fan-wei-lcof) | MEDIUM | 2 | 1 |
| 2020-06-29 05:00 | [#剑指 Offer 12 矩阵中的路径](https://leetcode-cn.com/problems/ju-zhen-zhong-de-lu-jing-lcof) | MEDIUM | 5 | 1 |
| 2020-06-24 09:05 | [#剑指 Offer 10- II 青蛙跳台阶问题](https://leetcode-cn.com/problems/qing-wa-tiao-tai-jie-wen-ti-lcof) | EASY | 1 | 1 |
| 2020-06-23 21:01 | [#剑指 Offer 07 重建二叉树](https://leetcode-cn.com/problems/zhong-jian-er-cha-shu-lcof) | MEDIUM | 1 | 1 |
| 2020-06-23 14:39 | [#剑指 Offer 06 从尾到头打印链表](https://leetcode-cn.com/problems/cong-wei-dao-tou-da-yin-lian-biao-lcof) | EASY | 4 | 1 |
| 2020-06-23 14:09 | [#剑指 Offer 05 替换空格](https://leetcode-cn.com/problems/ti-huan-kong-ge-lcof) | EASY | 1 | 1 |
| 2020-06-23 13:57 | [#剑指 Offer 04 二维数组中的查找](https://leetcode-cn.com/problems/er-wei-shu-zu-zhong-de-cha-zhao-lcof) | MEDIUM | 1 | 1 |
| 2020-06-23 08:43 | [#剑指 Offer 09 用两个栈实现队列](https://leetcode-cn.com/problems/yong-liang-ge-zhan-shi-xian-dui-lie-lcof) | EASY | 2 | **2** |
| 2020-06-22 13:41 | [#剑指 Offer 10- I 斐波那契数列](https://leetcode-cn.com/problems/fei-bo-na-qi-shu-lie-lcof) | EASY | 1 | 1 |
| 2020-06-22 10:03 | [#剑指 Offer 11 旋转数组的最小数字](https://leetcode-cn.com/problems/xuan-zhuan-shu-zu-de-zui-xiao-shu-zi-lcof) | EASY | 3 | 1 |
| 2020-05-26 07:57 | [#23 合并K个升序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists) | HARD | 1 | 1 |
| 2020-05-26 07:07 | [#21 合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists) | EASY | 1 | 1 |
| 2020-05-24 13:29 | [#138 复制带随机指针的链表](https://leetcode-cn.com/problems/copy-list-with-random-pointer) | MEDIUM | 1 | 1 |
| 2020-05-24 09:08 | [#142 环形链表 II](https://leetcode-cn.com/problems/linked-list-cycle-ii) | MEDIUM | 1 | 1 |
| 2020-05-24 08:16 | [#160 相交链表](https://leetcode-cn.com/problems/intersection-of-two-linked-lists) | EASY | 2 | 1 |
| 2020-04-03 21:56 | [#8 字符串转换整数 (atoi)](https://leetcode-cn.com/problems/string-to-integer-atoi) | MEDIUM | 3 | 1 |
| 2020-03-30 14:58 | [#剑指 Offer 03 数组中重复的数字](https://leetcode-cn.com/problems/shu-zu-zhong-zhong-fu-de-shu-zi-lcof) | EASY | 1 | 1 |
| 2020-03-30 14:15 | [#剑指 Offer 26 树的子结构](https://leetcode-cn.com/problems/shu-de-zi-jie-gou-lcof) | MEDIUM | 1 | 1 |
| 2020-03-30 12:09 | [#剑指 Offer 62 圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof) | EASY | 1 | 1 |
| 2020-02-15 13:56 | [#66 加一](https://leetcode-cn.com/problems/plus-one) | EASY | 1 | 1 |
| 2020-02-15 12:56 | [#35 搜索插入位置](https://leetcode-cn.com/problems/search-insert-position) | EASY | 2 | 1 |
