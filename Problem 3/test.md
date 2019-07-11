```java 
public class SolveProblem3 {
	public static void main(String[] args){
	long n = 600851475143L;
	
	int biggestPrime = 0;
    for(int i=2;i<n;i++){
		boolean prima=true;
        if(n%i==0){
           for(int j=2;j<i;j++){
				if(i%j==0){
					prima = false;
				}
			}
			if(prima==true){
				if(biggestPrime<i){
					biggestPrime = i;
				}
            }
		}

		if(i<0){
			break;
		}
	}
	System.out.println("Biggest prime factor from 600851475143 is = "+biggestPrime);

	}

}

```


