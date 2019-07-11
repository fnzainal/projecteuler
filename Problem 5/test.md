```java 
public class SolveProblem5 {
    public static void main(String[] args){
            int number = 1;
            boolean isTheTarget;

            while(true){
                isTheTarget = false;
                number++;
                for(int i=1;i<=20;i++){
                    if(number%i==0){
                        isTheTarget = true;
                    }else{
                        isTheTarget = false;
                        break;
                    }
                }

                if(isTheTarget){
                    System.out.println("The smallest positive number that is evenly divisible by numbers from 1 to 20 = "+number);
                    break;
                }
            }
    }

}

```


