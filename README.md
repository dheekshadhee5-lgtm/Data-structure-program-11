# Data-structure-program-11
#include <stdio.h>
#include <stdlib.h>
Struct Node {
 Char item[20];
 Struct Node* next;
};
Struct Node* head = NULL;
Void addItem(char name[]) {
 Struct Node* newNode = 
(struct 
Node*)malloc(sizeof(struct 
Node));
 Strcpy(newNode->item, 
name);
 newNode->next = head;
 head = newNode;
}
Void displayList() {
 Struct Node* temp = head;
 Printf(“Shopping List:\n”);
 While(temp != NULL) {
 Printf(“%s\n”, temp-
>item);
 Temp = temp->next;
 }
}
Int main() {
 addItem(“Milk”);
 addItem(“Bread”);
 addItem(“Eggs”);
 displayList();
 return 0;
}
>Shopping List:
Eggs
Bread
Milk
