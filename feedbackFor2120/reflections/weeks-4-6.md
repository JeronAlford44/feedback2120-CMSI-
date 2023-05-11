---
description: Jan 30–Feb 17

During these weeks we covered the "fun with arrays" program on leetcode.com, and learned a lot of different operations that can be used on an array. In addition, we started to dive into linked lists and their implementation. To learn this we used class discussions as well as the built-in leetcode lessons to help us.

Some sample code:

    Find Numbers with even number of digits:

                class Solution {
                    public int findNumbers(int[] nums) {
                        int count = 0;
                        for (int i = 0; i< nums.length; i++) {
                            String new_num = Integer.toString(nums[i]);
                            if (new_num.length() % 2 == 0){
                                count++;
                            }
                                
                        }
                        return count;
                    }
                }
    Linked List Cycle II:

public class Solution {
    public ListNode detectCycle(ListNode head) {
        ListNode fast;
        ListNode slow;
        ListNode prev;
        fast = head;
        slow = head;
      
        
        while (fast != null && fast.next != null){
           
            fast = fast.next.next;
            slow = slow.next;
            if (slow == fast){
                break;
            }
            
        }
        if (fast == null || fast.next == null) return null;
        while (head != slow) {
            head = head.next;
            slow = slow.next;
        }
        return head;
            
    }
}
---

# Weeks 4-6

