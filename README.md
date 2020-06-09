import java.util.Scanner;
class Main {
  public static void main(String[] args) {
    Scanner cin=new Scanner(System.in);
    int [] a=new int[6];
    while(cin.hasNext()){
      for(int i=0;i<6;i++){
        a[i]=cin.nextInt();
      }
      for(int i=0,n=0;n<200001;i++){ //<=200000
        n=a[0]*i+a[1];
        if(judge(n-a[3],a[2])){ //第二個是否符合?
          if(judge(n-a[5],a[4])){ //第三個是否符合?
            System.out.println(n);
            break;
          }
        }
      }
    }
  }
  static boolean judge(int n,int x){ //判斷是否可整除   
    if((n/x*x)==n) return true;
    else return false;
  }
}
