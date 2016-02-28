#Sample Definitions of some Data Structures and Algorithms (Java):

##I. Data Structires:

##Linked Lists
Each node in a linked list has a data element and a pointer to the next node:

```java
		class LLNode {
		int data;
		LLNode next;
		
		LLNode(int data) {
			this.data = data;
		  }
		}
```


##Double linked Linked List :
means that each node has a pointer to the previous node as well. A sample definition would be:

```java
  class DLLNode {
		int data;
		DLLNode next, prev;
		
		DLLNode(int data) {
			this.data = data;
		}
	}
```


Time Complexity:
insert is O(1)
look up is O(n)

## Binary trees : have only two children  :

```java
	class TNode {
		int data;
		TNode left, right;
		
		TNode(int data) {
			this.data = data;
		}
	}
```


## Binary Search Tree:
Each node element in the tree must be greater than every element on it's left and less than the elements on it's right.
The process of visiting each node in a tree is called tree traversal. There are three basic ways to explore a tree in a depth-first order. The following sample code prints a tree with the three basic traversals:
	
```java
		public static void preOrder(TNode root) {
		if (root == null) { return; };
		System.out.println(root.data);		
		preOrder(root.left);
		preOrder(root.right);
		}
```


**In order**

```java
		public static void inOrder(TNode root) {
		if (root == null) { return; };
		inOrder(root.left);
		System.out.println(root.data);
		inOrder(root.right);
		}
```
	
**Post Order**

```java
		public static void postOrder(TNode root) {
		if (root == null) { return; };
		postOrder(root.left);
		postOrder(root.right);
		System.out.println(root.data);
		}
```


##Hash Tables
A hash map is used to associate a key with a value
theoretically each operation (insertion, removal, look-up) requires on average O(1) time

`HashMap<String, String> hm = new HashMap<String, String>();`

##Stack
A Last-in-First-Out daata structure
`Stack<String> stack = new Stack <String>();`

##Queues
A First-In-First-Out data structure
`Queue<String> queue = new LinkedList<String>();`

##Graph
A set of nodes that are connected by links, represented using an adjacency matrix or an adjacency list.


##II. Algorithms:
