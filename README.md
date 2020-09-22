<div align="center">

## A Simple Bubble Sort


</div>

### Description

Sorts a pre-definied array into order. My second submission under the C++ section, and my second day of learning this language..so go easy :)
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Brutus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/brutus.md)
**Level**          |Beginner
**User Rating**    |3.9 (27 globes from 7 users)
**Compatibility**  |Microsoft Visual C\+\+
**Category**       |[Sorting](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/sorting__3-24.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/brutus-a-simple-bubble-sort__3-2966/archive/master.zip)





### Source Code

```
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
```

