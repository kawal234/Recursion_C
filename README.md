# Recursion_C

#include<stdio.h>

// Factorial by recursion
/*
int factorial(int n){
	if (n==1|| n==0){
		return 1;
	}else{
		return n*factorial(n-1);
	}
	
}

int main(){
	int a;
	printf("Enter the Number : ");
	scanf("%d",&a);
	int fact = factorial(a);
	printf("%d",fact);
	return 0;
}

---------------------------------------------------------------------------------------------------------------------

// Printing Numbers from n to 1

void decresing(int n){
	if(n==0) return;
	printf("%d\n",n);
	decresing(n-1);
	return;
}


int main(){
	int a;
	printf("Enter the Number : ");
	scanf("%d",&a);
	decresing(a);
	return 0;
}


-------------------------------------------------------------------------------------------------------------------------------------

show the sum of the numbers from n to 0
void Sum(int n,int count=0){
	if (n==0){
		printf("The Sum of the Numbers are : %d",count);
		return;
	}
	Sum(n-1,count+n);
	return ;
	
}

int main(){
	int a;
	printf("Enter the Number : ");
	scanf("%d",&a);
	Sum(a);
	return 0;
}


-----------------------------------------------------------------------------------------------------------

to print the power of a number

int power(int a,int b){
	if(b==0) return 1;
	return a*power(a,b-1);
}

int main(){
	int a,b;
	printf("Enter base and power : ");
	scanf("%d %d",&a,&b);
	int p = power(a,b);
	printf("The Answer is : %d",p);
	return 0;
}

 
-----------------------------------------------------------------------------------------------------------

// Print Fibonacci Pattern
int fibo(int n){
	if(n==1||n==2) return 1;
	return fibo(n-1)+fibo(n-2);
}

int main(){
	int a;
	printf("Enter the Number : ");
	scanf("%d",&a);
	printf("%d",fibo(a));
	return 0;
}

------------------------------------------------------------------------------------------------------------------

// Stair Path-1

int stair(int n){
	  if(n==0) return 1;
	  else if(n<0) return 0;
	  return stair(n-1)+stair(n-2)+stair(n-3);
}
int main(){
	int a;
	printf("Enter the Number of Stairs : ");
	scanf("%d",&a);
	printf("%d",stair(a));
	return 0;
} 

-------------------------------------------------------------------------------------------------------------------------------

// Poweerlog By Recursion
int powerlog(int a,int b){
	if (b==0) return 1;
	if(b%2==0) return powerlog(a,b/2)*powerlog(a,b/2);
	return powerlog(a,b/2)*powerlog(a,b/2)*a;
}

int main(){
	int a,b;
	printf("Enter base and power : ");
	scanf("%d %d",&a,&b);
	int p = powerlog(a,b);
	printf("The Answer is : %d",p);
	return 0;
}

-----------------------------------------------------------------------------------------------------------------

// Maze path - 1
int maze(int cr,int cc,int er,int ec ){
	int Rightw =0;
	int Leftw =0;
	if(cr==er && cc==ec) return 1;
	if (cr==er){//Only right ways
		Rightw += maze(cr,cc+1,er,ec);
	}
	if(cc==ec){// only left ways
		Leftw += maze(cr+1,cc,er,ec);
	}
	if(cr<er && cc<ec){
		Rightw += maze(cr,cc+1,er,ec);
		Leftw += maze(cr+1,cc,er,ec);
	}
	
	int totalW = Rightw+ Leftw;
	return totalW;
}

int main(){
	int a,b;
	printf("Enter rows and columns : ");
	scanf("%d %d",&a,&b);
	int w = maze(1,1,a,b);
	printf("The Maze Would be : %d",w);
	return 0;
}

-------------------------------------------------------------------------------------------------------------------------------

//Maze Path -2 
int maze2(int n,int m){
	int Rightw =0;
	int Leftw =0;
	if(n==1 && m==1) return 1;
	if(n==1){
		Rightw += maze2(n,m-1);
	}
	if(m==1){
		Leftw += maze2(n-1,m); 
	}
	else{
		if(n>1&&m>1){
			Rightw += maze2(n,m-1);
			Leftw += maze2(n-1,m);
		}
	}
	int totalW = Rightw+ Leftw;
	return totalW;
}


int main(){
	int a,b;
	printf("Enter rows and columns : ");
	scanf("%d %d",&a,&b);
	int w = maze2(a,b);
	printf("The Maze Would be : %d",w);
	return 0;
}

-------------------------------------------------------------------------------------------------------------------

// Code for Printing PreInPost Pattern
void zigzag(int n){
	if(n==0) return;
	printf("%d",n);
	zigzag(n-1);
	printf("%d",n);
	zigzag(n-1);
	printf("%d",n);
	return ;
	
}

int main(){
	int a;
	printf("Enter the Number : ");
	scanf("%d",&a);
	printf("%d",zigzag(a));
	return 0;
}

------------------------------------------------------------------------------------------------------------------------------

// Tower of Hanoi
void tower(int n, char s,char h,char d){
	if(n==0) return;
	tower(n-1,s,d,h);
	printf("%c --> %c\n",s,d);
	tower(n-1,h,s,d);
	return;
}

int main(){
	int a;
	printf("Enter the Number of disks : ");
	scanf("%d",&a);
	tower(a,'A','B','C');
	return 0;
}
*/

===============================================================================================================================================================
