![![# CC-2-exp8 (24BDA70130) 
## Problem Statement:328. Odd Even Linked List 
class Solution: 
 
    def oddEvenList(self, head): 
        if not head or not head.next: 
            return head 
        odd = head 
        even = head.next 
        evenHead = even 
        while even and even.next: 
            odd.next = even.next mplete installation. Please approve the UAC prompt, then send me a message and I’ll initialize the repository, commit the files, and push 
            odd = odd.next 
            even.next = odd.next 
            even = even.next 
        odd.next = evenHead 
        return head ](image-1.png)](image.png)