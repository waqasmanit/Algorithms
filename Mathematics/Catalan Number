/* Source: 
 video : https://www.youtube.com/watch?v=eoofvKI_Okg
  
 video: https://www.youtube.com/watch?v=CMaZ69P1bAc
 
 Applications :  https://www.geeksforgeeks.org/applications-of-catalan-numbers
 
 Over 200 questions on Catalan number   : http://math.mit.edu/~rstan/ec/
 
 Good read:    https://www.geeksforgeeks.org/program-nth-catalan-number/
              
 */

//dp solution with O(n*n) complexity

#define MOD 1000000007;

long long int catalanDP(unsigned int n) 
{ 
long long int dp[n+1];
    if(n==0||n==1)
     return 1;
    else if(n==2)
     return 2;
    else if(n>2){
        dp[0]=1;
        dp[1]=1;
        dp[2]=2;
        for(int i=3;i<=n;i++){
            dp[i]=0;
            for(int k=0;k<i;k++){
                dp[i]=(dp[i]+dp[i-k-1]*dp[k])%MOD;
            }
        }
       
    }
     return dp[n]%MOD;
}

