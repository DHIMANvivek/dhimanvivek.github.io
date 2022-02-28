# 1

# Sum Pattern 

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->



#### Code you used for Submit/Run operation


```
// Sum Pattern
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int n = s.nextInt();
        int currRow = 1;
        int sum = 0;
        while(currRow <= n) {
            sum += currRow;
            int currCol = 1;
            while(currCol <= currRow) {
                System.out.print(currCol);
                if(currCol == currRow)
                	System.out.print("=");
                else
                	System.out.print("+");
                currCol += 1;
            }
            System.out.println(sum);
            currRow += 1;
        }
    }
}
```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
milestone 1 pattern-2

#### Screenshots

![sum pattern](https://user-images.githubusercontent.com/53940939/155983142-287d0dfd-f055-4d6a-90ee-8719777a0ead.png)

# 2

# Parallelogram Pattern

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Main {
	
	public static void main(String[] args) {
        Scanner s = new Scanner (System.in);
		int n = s.nextInt();
		
		
		
		int i = 1;
		
		while(i<=n) {
			int space = 1;
			while(space<=i-1) {
				System.out.print(" ");
				space = space + 1;
				
			}
			int j = 1;
			while (j<= n) {
				System.out.print("*");
				j = j + 1;
				
			}
			
			i = i + 1;
			System.out.println();
		}
		// Write your code here

	}
}

```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Parallelogram Pattern


#### Screenshots


![parallelogram](https://user-images.githubusercontent.com/53940939/155984582-9014f83a-5a92-4edc-bf9d-25094f98f952.png)


# 3

# Half Diamond Pattern

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Solution {
    
     public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		int n = scan.nextInt();
		int i = 1;
		int n1 = n;
		int n2 = n1-1;
		
		System.out.println("*");
		while (i <= n1) {

			
			int star = 1;
System.out.print("*");
			while (star <= i) {
				// i+j-1;
				System.out.print(star);
				star++;
			}
			int dec = i - 1;
			while (dec >= 1) {
				System.out.print(dec);
				dec--;
			}
			System.out.print("*");
			System.out.println();
			i++;

		}

		i = n2;

		while (i > 0) {
			System.out.print("*");
			int star = 1;

			while (star <= i) {
				// i+j-1;
				System.out.print(star);
				star++;
			}
			int dec = i - 1;
			while (dec >= 1) {
				System.out.print(dec);
				dec--;
			}
			System.out.print("*");
			System.out.println();
			i--;

		}
		System.out.print("*");
	}
}

```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
 Half Diamond Pattern


#### Screenshots


![half diamond](https://user-images.githubusercontent.com/53940939/155985151-811353de-1999-4759-be03-b3748d9eb814.png)


# 4

# Star Diamond Pattern

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Solution {
    
   public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		int n = scan.nextInt();
		int i = 1;
		int n1 = (n + 1) / 2;
		int n2 = n / 2;
		while (i <= n1) {

			int j = n1;
			while (j <= n - i) {
				System.out.print(" ");
				j++;
			}
			int star = 1;

			while (star <= i) {
				// i+j-1;
				System.out.print("*");
				star++;
			}
			int dec = i - 1;
			while (dec >= 1) {
				System.out.print("*");
				dec--;
			}
			System.out.println();
			i++;

		}

		i = n2;

		while (i > 0) {
			int space = n2 + 1;

			while (space <= n - i) {
				System.out.print(" ");
				space++;
			}
			int star = 1;

			while (star <= i) {
				// i+j-1;
				System.out.print("*");
				star++;
			}
			int dec = i - 1;
			while (dec >= 1) {
				System.out.print("*");
				dec--;
			}
			System.out.println();
			i--;

		}
	}
}
```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
 Star Diamond Pattern


#### Screenshots


![Diamond Pattern](https://user-images.githubusercontent.com/53940939/155985506-39d9bf40-f716-4115-a37b-fe442b4d2fed.png)



# 5

# Triangle of Numbers

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;

public class Solution {

	public static void main(String[] args) {
		/* Your class should be named Solution.
	 	* Read input as specified in the question.
	 	* Print output as specified in the question.
		*/
	Scanner scan = new Scanner(System.in);
		int n = scan.nextInt();
		int i = 1;

		while (i <= n) {

			int j = 1;
			while (j <= n - i) {
				System.out.print(" ");
				j++;
			}
			j = 1;
			int r = i;
			while (j <= i) {
				System.out.print(r);
				r++;
				j++;

			}

			r = r - 2;
			j = 1;
			while (j <= i - 1) {
				System.out.print(r);
				r--;
				j++;
			}
			System.out.println();
			i++;

		}

	}

}

```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Triangle of Numbers


#### Screenshots


![pattern of numbers](https://user-images.githubusercontent.com/53940939/155985810-9e7c7371-b82c-48d0-bbc2-8f42ef9d290b.png)


# 6

# Character Pattern

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Solution {


	public static void main(String[] args) {
		char a = 'A';

		Scanner scan = new Scanner(System.in);

		int s = scan.nextInt();
		int i = 1;
		while (i <= s) {

			int j = 1;
			char ab = (char) ('A' + i - 1);
			while (j <= i) {

				System.out.print(ab);
				// a = (char) (a+1);
				// a=(char)(a+1);
				ab = (char)(ab+1);
				j += 1;

			}
			System.out.println();

			i++;

		}

	}

}


```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Character Pattern


#### Screenshots


![character pattern](https://user-images.githubusercontent.com/53940939/155986279-d6f5aaca-4e30-4771-a680-427d6ab24d9c.png)


# 7

# Reverse Number Pattern

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Solution {


	public static void main(String[] args) {
		 		Scanner scan = new Scanner(System.in);
		int n = scan.nextInt();
		int i = 1;

		while (i <= n) {
			int j = 1;

			while (j <= i) {

			
				
                System.out.print((i+1)-j);
				j = j+1;
				

			}
			System.out.println();
			 i++;

            

		}

	}

}


```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Reverse Number Pattern


#### Screenshots


![reverse number](https://user-images.githubusercontent.com/53940939/155986598-a3319c43-bedc-4df3-9a15-1ffedb5277eb.png)




# 8

# Odd Square

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->


#### Code you used for Submit/Run operation


```
// Pattern 
import java.util.Scanner;
public class Main {
	
	public static void main(String[] args) {
		// Write your code here
        Scanner s=new Scanner(System.in);
        int n=s.nextInt();
        for(int i=1;i<=n;i++){
            for(int j=i-1;j<n;j++){
                System.out.print(j*2+1+"");
            }
            for(int k=0;k<i-1;k++){
                System.out.print(k*2+1);
            }
            System.out.println();
        }
      //  int count=0;
        // for(int i=0;i<n;i++){
        //    // int count=0;
        //     for(int j=0;j<2*n;j++){
        //         if(j%2!=0){
        //              System.out.print(j+count);
        //         }
        //        // count++;
        //     }
        //     // for(int j=0;j<n;j++){
        //     //     System.out.print(i+j+1);
        //     // }
        //     System.out.println();
        //     count=count+2;
        
	}
}



```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
Odd Square


#### Screenshots


![odd square](https://user-images.githubusercontent.com/53940939/155987279-afa24041-a764-495a-8d57-ce46c7e3e3fd.png)













