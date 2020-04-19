# pattern28







import java.util.*;
class Main{
  public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    int n = sc.nextInt();
    int nsp = n-1;
    int nst = 1;
    
    //row
    int row = 1;
        while(row<= n){
             int val = row;
      // work space
    int csp = 1;
    while(csp<= nsp){
      System.out.print(" ");
      csp++;
    }
      
      //work Star
    int cst = 1;
    while(cst<= nst){
       System.out.print(val);
       if(cst <= nst/ 2)
       {
           val++;
       }
           else{
               val--;
           }
       
       cst++;
    }
       System.out.println();
       row = row +1;
       nsp = nsp - 1;
       nst = nst + 2;
    }
    
  }
}
