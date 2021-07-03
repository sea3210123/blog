age imooc;

public class a1 {

	 public static void main(String[]args) {
		 int n1=12;int n2=3;
		 int r;
		 //加法
		 r=n1+n2;
		 System.out.println(n1+"+"+n2+"="+r);
		 //减法
		 r=n1-n2;
		 System.out.println(n1+"-"+n2+"="+r);
		 //乘法
		 r=n1*n2;
		 System.out.println(n1+"*"+n2+"="+r);
		 //除法
		 r=n1/n2;
		 System.out.println(n1+"/"+n2+"="+r);
		 //分子分母为整型时，得结果无余数
		 System.out.println(13/5);
		 System.out.println(13.0/5);
		 //余数
		 r=45%n2;
		 System.out.println("45"+"%"+n2+"="+r);
		  
		 int x;x=4;
		 int y;y=(x++)+5;
		 System.out.println("x="+x+" y="+y);
		 x=4;y=(++x)+5;
		 System.out.println("x="+x+" y="+y);
		//++x先自增后运算  x++反之
		 //--x同理
	 }
	 
}
package imooc;

public class a2 {
	public static void main(String[]args) {
		int a=3,b=9;
		System.out.println("a<b="+(a<b));
		System.out.println("a>b="+(a>b));
	
		int price1,price2;
		price1=34;price2=98;
		int sum=price1+price2;
		System.out.println("sum1="+sum);
		if(sum>100) {
			sum-=20;//sum=sum-20;
			System.out.println("sum2="+sum);
		}
	int n=9;
	if(n%2==0) {
		System.out.println(n+"为偶数");}
else {System.out.println("n为奇数");}
	
	
	}
	

}

