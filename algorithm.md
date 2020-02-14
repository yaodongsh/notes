## link list
* Reverse
	* create 3 nodes. Cur, Prev and Next (used to save Next)
	>
        Node* cur=head;    
        Node* prev=NULL;
        next;
        while (cur != NULL)
        {
                next=cur->next; //save cur->next
                cur->next=prev; //reverse, make cur->next point to prev
                prev=cur;       //before cur point to next, make prev = cur;
                cur=next;       //iter to next node, use saved 
        }
        return prev;        //this is actual cur before NULL

