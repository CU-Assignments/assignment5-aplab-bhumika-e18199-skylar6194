class Solution {
public:
    TreeNode* prev;

    bool isValidBST(TreeNode* root) {
        prev = nullptr;
        return dfs(root);
    }

    bool dfs(TreeNode* root) {
        if (!root) return true;
        if (!dfs(root->left)) return false;
        if (prev && prev->val >= root->val) return false;
        prev = root;
        if (!dfs(root->right)) return false;
        return true;
    }
};
