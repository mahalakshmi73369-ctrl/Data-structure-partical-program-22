# Data-structure-partical-program-22
Inorder Traversal
Left → Root → Right

class Node:
    def __init__(self, data):
        self.left = None
        self.right = None
        self.data = data

def inorder(root):
    if root:
        inorder(root.left)
        print root.data,
        inorder(root.right)

# Create nodes
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)
root.left.right = Node(5)

print "Inorder Traversal:"
inorder(root)
