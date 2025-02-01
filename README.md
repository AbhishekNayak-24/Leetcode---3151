# Leetcode---3151
Special Array I
//CODE IN JAVA
public class Solution {
    public boolean isArraySpecial(int[] nums) {
        for (int i = 1; i < nums.length; i++) {
            if (nums[i] % 2 == nums[i - 1] % 2) {
                return false;
            }
        }
        return true;
    }

    public static void main(String[] args) {
        Solution solution = new Solution();
        int[] nums1 = {1, 2, 3, 4};
        int[] nums2 = {1, 3, 5, 7};
        System.out.println(solution.isArraySpecial(nums1)); // Output: true
        System.out.println(solution.isArraySpecial(nums2)); // Output: false
    }
}
