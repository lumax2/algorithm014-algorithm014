学习笔记
学习总结：
参与14期算法训练营，目前收获感最强烈地方如下：
1 leetcode 的使用；intelliJ leetcode plugin插件；
2 算法知识结构梳理；思维导图，增加了对算法结构的认识；
3 五毒大法 职业化的训练思路 很受启发；

具体：比如 移动零 这种双指针思维方式，很有启发
class Solution {
    public void moveZeroes(int[] nums) {
        if (nums == null) {
            return;
        }
        int j = 0;
        for (int i = 0; i < nums.length; ++i) {
            if (nums[i] != 0) {
                nums[j++] = nums[i];
            }
        }
        for (int i = j; i < nums.length; ++i) {
            nums[i] = 0;
        }

    }
}