# Finding middle element in a linked list
# Given a singly linked list of N nodes.
# The task is to find the middle of the linked list. For example, if the linked list is
# 1-> 2->3->4->5, then the middle node of the list is 3.
# If there are two middle nodes(in case, when N is even), print the second middle element.
# For example, if the linked list given is 1->2->3->4->5->6, then the middle node of the list is 4.
# -------------------------------------------------------------------------------------------------------------------------

#Creating the Node
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
#Initialising the Head as None
    def __init__(self):
        self.head = None
#Creating the method to insert elements in LinkedList
    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
            return
        current_node = self.head
        while current_node.next is not None:
            current_node = current_node.next
        current_node.next = new_node

#Creating the method to find the Middle element of the LinkedList
    def find_Mid(self, head):
        if head is None:
            return None
        slow = head
        fast = head 
        while fast is not None and fast.next is not None:
            slow = slow.next
            fast = fast.next.next
        return slow.data
        
#Creating LinkedList object

my_List = LinkedList()
my_List.append(1)
my_List.append(2)
my_List.append(3)
my_List.append(4)
my_List.append(5)
print(my_List.find_Mid(my_List.head))
#----------------------------------------------------------------END -------------------------------------------------------------------
