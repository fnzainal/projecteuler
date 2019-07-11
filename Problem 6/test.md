```java 
public class SolveProblem6 {
	public static void main(String[] args){

        int sumSquare = 0;
        int squareOfSum = 0;
        int sumOfHundred = 0;

        for(int i=1;i<=100;i++){
            sumSquare = sumSquare+(i*i);
            sumOfHundred = sumOfHundred+i;
        }

        squareOfSum = sumOfHundred*sumOfHundred;
        int result = squareOfSum-sumSquare;

        System.out.println("Difference between the sum of the squares of the first one hundred natural numbers and the square of the sum: ");
	    System.out.println(+squareOfSum+" - "+sumSquare+" = "+result);
	}

}
```


