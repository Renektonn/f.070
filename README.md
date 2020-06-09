class Main {
  public static void main(String[] args) {
    int a1=3,a2=2,b1=5,b2=3,c1=7,c2=2;
    for(int i=0,n;true;i++){
      n=a1*i+a2;
      if(judge(n-b2,b1)){

      }
    }
  }
  static boolean judge(int n,int x){   
    if((n/5*5)==n) return true;
    else return false;
  }
}
