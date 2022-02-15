#include<stdio.h>

#define SIZE 1

Void enQueue(int);

Void deQueue();

Void display();

Int items[SIZE],front=-1,rear=-1;

Int main()

{

    deQueue();

    enQueue(1);

    enQueue(2);

    display();

    deQueue();

    display();

    return 0;

}

Void enQueue(int value)

{

    If(rear==SIZE-1)

    Printf(“\nable to access the printer!!”);

    Else

    {

        If(front==-1)

        Front=0;

        Rear++;

        Items[rear]=value;

        Printf(“\ndoes not able to access the printer->%d”,value);

    }

}

Void deQueue()

{

    If(front==-1)

    Printf(“\ndoes not able to access the printer!!”);

    Else

    {

        Printf(“\nable to access the printer:%d”,items[front]);

        Front++;

        If(front>rear)

        Front=rear=-1;

    }

}

Void display()

{

    If(rear==-1)

    Printf(“\nable to access the printer!!!”);

    Else

    {

        Int i;

        Printf(“\n printer gives access to first person only:\n”);

    For(i=front;i<=rear;i++)

    Printf(“%d”,items[i]);

}

Printf(“\n”);

}
