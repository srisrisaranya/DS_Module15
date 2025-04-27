# Ex12 Binary Search Tree
## DATE:
## AIM:
To write a C function to insert the elements in the binary search tree

## Algorithm
```
1.	Start
2.	Check if the current node is NULL; if true, create a new node with the given key.
3.	Allocate memory for the new node, set its key, and initialize its left and right children to NULL.
4.	If the current node is not NULL, compare the key with the current node's key.
5.	If key <= node->key, recursively insert the key into the left subtree and update the left child pointer.
6.	If key > node->key, recursively insert the key into the right subtree and update the right child pointer.
7.	Return the current node after the insertion.
8.	End

```
## Program:
```
/*
Program to insert the elements in the binary search tree
Developed by: SARANYA S
RegisterNumber:  212223110044
*/
```
```
/*struct node {
   int key;
   struct node *left, *right;
};*/
struct node* insert(struct node* node, int key) {
    //type your code here
    if(node==NULL)
    {
        return newNode(key);
    }
    if(key<node->key)
    {
        node->left=insert(node->left,key);
        
    }
    else if(key>node->key)
    {
        node->right=insert(node->right,key);
    }
    return node;
}
```
## Output:
![image](https://github.com/user-attachments/assets/98eba7d5-3274-4849-870f-344036cf9c54)

## Result:
Thus, the C function to insert the elements in the binary search tree is implemented successfully.
