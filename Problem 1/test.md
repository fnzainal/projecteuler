```java 
public class SolveProblem1 {
	public static void main(String[] args){
	int total = 0;
	for(int i=0;i<1000;i++){
            if(i%3==0 || i%5==0){
                total = total+i;                
              }
		}
		System.out.println("Sum of all the multiples of 3 or 5 below 1000 = "+total);
        // result print should : Sum of all the multiples of 3 or 5 below 1000 = 233168
	}
}
```


