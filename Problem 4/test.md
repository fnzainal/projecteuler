```java 
public class SolveProblem4 {
    public static void main(String[] args){
            int number = 100;
            int multipleBy = 0;
            int largestPalindrome = 0;

            int largestX = 0;
            int largestY = 0;

            int result = 0;
            while(number<=999 && multipleBy<=999){
                for(int i=100;i<999;i++){
                    result = number*i;
                    multipleBy= i;

                    String sresult = String.valueOf(result);
                    int lenghtResult = sresult.length();
                    
                    if(lenghtResult%2==0){
                        String begind = sresult.substring(0, lenghtResult/2);
                        String end = sresult.substring(lenghtResult/2);
                        StringBuilder sb = new StringBuilder(end);

                        if(begind.equals(sb.reverse().toString())){
                            largestX = number;
                            largestY = i;

                            // set the largest palindrom
                            if(result>largestPalindrome){
                                largestPalindrome = result;
                            }
                        }
                    }
                }
                number++;
            }
            System.out.println("Largest palindrome number by the product of two 3-digit numbers : "+largestX+"*"+largestY+" = "+largestPalindrome);
    }

}


```


