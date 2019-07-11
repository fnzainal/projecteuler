```java 
public class SolveProblem2 {
        public static void main(String[] args){
                int a = 0;
                int b = 1;
                int result = 0;
                int total = 0;

                while(result<4000000){
                    result = a+b;
                    if(result%2==0){
                        total = total+result;
                    }

                    a = b;
                    b = result;
                }
                
                System.out.println("");
                System.out.println("Sum of the even-valued terms under 4000000 = "+total);

        }

}
```


