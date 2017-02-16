/*The structure of linked list is the following
struct Node
{
int data;
Node* next; 
};*/

/*The function removes the loop from the linked list if present
You are required to complete this method*/
void removeTheLoop(Node *node)
{
     //Your code here
     Node *slow,*fast;
     slow=node,fast=node->next;
     while(fast && fast->next)
     {
         slow=slow->next;
         fast=fast->next->next;
         if(slow==fast)
            break;
     }
     
     if(slow==fast)
     {
        slow=node;
        while(fast->next!=slow)
        {
            slow=slow->next;
            fast=fast->next;
        }
        fast->next=NULL;
     }
}
