### Hi there 👋

Here are some ideas to get you started:

- 🔭 I’m currently working on python modules
- 🌱 I’m currently learning machine learning
- 👯 I’m looking to collaborate on machine learning projects
- 🤔 I’m looking for help with backpropogation
- 💬 Ask me about python
- 📫 How to reach me: you can't :P
- 😄 Pronouns: He/Him
- ⚡ Fun fact: I am iron man




#include<stdio.h>
#include<conio.h>

#define size 10

void append(int a[], int *n, int x)
{
	if(*n<size)
	{
	a[*n]=x;
	(*n)++;
    }
}

void Display(int a[], int n)
{
	int i=0;
		printf("Elements of array are: ");
		for(i=0; i<n; i++)
		{
			printf("%d ", a[i]);
		}
		
}


int main()
{
	int n, m, i=0;
	int arr[size];
	printf("Enter the no of elements:\n");
	scanf("%d", &n);
	printf("Enter the elements of the array:\n");
	for(i=0; i<n; i++)
	{
		scanf("%d", &arr[i]);
	}
	printf("Enter the element you want to add:");
	scanf("%d", &m);
	Display(arr, n);
	append(arr, &n, m);
	printf("\n");
	Display(arr, n);
	
	return 0;
	
}
