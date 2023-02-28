# N 叉树的前序遍历

```javascript
let preorder = function (root) {
  let res = [];
  function traversal(root) {
    if (root) {
      res.push(root.val);
      res.children.forEach((item) => traversal(item));
    }
  }
  traversal(root);
  return res;
};
```

# N 叉树的后序遍历

```javascript
let preorder = function (root) {
  let res = [];
  function traversal(root) {
    if (root) {
      res.children.forEach((item) => traversal(item));
      res.push(root.val);
    }
  }
  traversal(root);
  return res;
};
```
