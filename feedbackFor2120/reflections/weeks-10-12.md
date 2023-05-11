---
description: Mar 20–Apr 7
During these weeks we took a deep dive in to different tree structures, and their difference in definition and applicability. THe main types we covered so far in these weeks included the binary tree, binary search tree, and full tree. We drew the different types of trees on paper and we also questioned on identifying the specific tree structure based on the layout of their nodes. We learned how to implement the binary search tree both iteratively and recursively. I like the recursive approach better, since i think in this case its a little easier to follow along with

code: class Solution {
  public TreeNode insertIntoBST(TreeNode root, int val) {
    if (root == null) return new TreeNode(val);

    // insert into the right subtree
    if (val > root.val) root.right = insertIntoBST(root.right, val);
    
    // insert into the left subtree
    else root.left = insertIntoBST(root.left, val);
    return root;
  }
}
---

# Weeks 10-12

