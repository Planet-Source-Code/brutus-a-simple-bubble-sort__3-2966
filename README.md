<div align="center">

## A Simple Bubble Sort<br/>by Brutus


</div>

### Description

Sorts a pre-definied array into order. My second submission under the C++ section, and my second day of learning this language..so go easy :)
 

 






### Source Code

#include <iostream.h>
#include <string.h>
#include <conio.h>
	//jumbled up text in array
	char strarray[] = "fgjhsflsdlkfghdksdkjdgskakdkfkjggkdkgjg";
	int i = 0;
	int j = 0;
	char temp;
	void Bubble(char* strarray, int arrsize);
	
int main()
{
  cout << strarray << endl;
  Bubble(strarray, strlen(strarray));
  cout << strarray << endl;
	
return 0;
}
	
void Bubble(char* strarray, int arrsize) //Bubble Sort code
{
	for(i=0; i< (arrsize - 1); ++i)
	{
		for(j = i + 1; j > 0; --j)
		{
			if(strarray[j] < strarray[j-1])
			{
				//Swaps the values
				temp = strarray[j];
				strarray[j] = strarray[j - 1];
				strarray[j - 1] = temp;
			}
			
		}
	}
}
