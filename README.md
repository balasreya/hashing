# hashing



#include<stdio.h>
#define size 10
void init(int arr[])
{
        int i;
        for(i=0;i<size;i++)
        {
                arr[i]=0;
        }

}
void insert(int arr[])
{
        int ch;
        do
        {
                int key;
                printf("enter the key value to be inserted");
                scanf("%d",&key);
                int value=key%size;
                if(arr[value]==0)
                {
                arr[value]=key;
                }
                else
                {
                printf("collision is occured");
        printf("arr[%d]is alredy has %d",value,key);
                }
        printf("enter 1-continue\n,0-exist\n");
        scanf("%d",&ch);
        }
while(ch==1)
}
void delete(int arr[])
{
        int ch;
        do
        {
                int key;
                printf("enter the key value to be deleted");
                scanf("%d",&key);
                int value=key%size;
                if(arr[value]==key)
                {
                        arr[value]=0;
                }
                else
                {
                        printf("value is not found");
                }
                printf("enter 1-continue\n,0-exist\n");
                scanf("%d",&ch);
        }
        while(ch==1)
}
void search(int arr[])
{
        int ch;
        do
        {
                int key;
                printf("enter the key value to be searched");
                scanf("%d",&key);
                int value=key%size;
                if(arr[value]==key)
                {
                        printf("value is found");
                }
                else
                {
                        printf("value is not found");
                }
        }
}
void print(int arr[])
{
        int i;
        for(i=0;i<size;i++)
        {
                arr[value]=key;
        }
}
int main()
{
        int arr[size];
        int choice=0;
        while(choice<5)
        printf("enter 1-insert\n,2-delete\n");
        printf("enter 3-search\n");
        printf("enter 4-print\n");
        peintf("enter the choice");
        scanf("%d",&choice);
        switch(choice)
        {
                case 1:
                        insert();
                        break;
                case 2:
                        delete();
                        break;
                case 3:
                        search();
                        break;
                case 4:
                        print();
                        break;
                case 5:
                        printf("enter wrong choce");
                        break
        }
}
