public class BitwiseFastExponential {
    public static int FastExpo(int a, int n){
        int answer =1;
        while(n>0){
        if((n&1)!=0){
            answer =answer*a;
        }
        a=a*a;
        n=n>>1;
        }
    return answer;
    }
public static void main(String[] args) {
    System.out.println(FastExpo(5, 3));
}
}
