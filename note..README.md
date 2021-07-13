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
		 7.5
		 {package imooc;
import java.util.Scanner;
public class a0705 
	//运算符的优先级
	//()>>!,++,-->>*，/，%》》+,-》》<,<=》》
    //==，!=》》&&》》||》》=，+=，*=，/=，-=，%=
	public static void main(String[]args) {
	int n=4,m=8;
	int v=(n--)+(n/m)*n;
	System.out.println("v="+v+n);
	//v=43      4/8=0
	//判断是否为闰年
	  System.out.println("请输出一个年份");
	    Scanner sc=new Scanner(System.in);
	    int a=sc.nextInt();
	    //if(a%400==0) 
	    	if((a%4==0)&(a%100!=0)|(a%400==0))
	    {System.out.println(a+"为闰年");}
	    else {System.out.println(a+"不是闰年");}
	    
	}
	
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
7.4	
package imooc;
import java.util.Scanner;//
public class a0704 {
	public static void main(String[]args) {
		
		  //逻辑运算符  布尔类型
		    //与  &  &&(&运算两个条件，&&如果运算一不满足，运算二不运算，值为false)    operator1||operator2
		    //或  |  ||      operator1||operator2（同上）
		   // 非  !       !operator
		int a=4;
	boolean b=((a--)>(a+3))&(3<(a--));
    System.out.println("a="+a+" "+"b="+b);
    //a=2 b=false
    int c=4;
    boolean d=((c--)>(c+3))&&(3<(c--));
    System.out.println("c="+c+" "+"d="+d);
    //c=3 d=false
    int e=4;
    boolean f=((++e)>4)|(4>6);
    System.out.println("e="+e+" "+"f="+f);
    //e=5 f=true
    int g=5;
    boolean h=(6<9)||((g--)<7);
    System.out.println("g="+g+" "+"h="+h);
    //g=5 h=true
    System.out.println("请输出一个整数");
    Scanner sc=new Scanner(System.in);
    int n=sc.nextInt();
    if(!(n%4==0)){
    	System.out.println(n+"不为4的倍数");
    }else {System.out.println(
    	n+"是4的倍数");
    }
   //请输出一个整数
   // 52
   //52是4的倍数
   
   //条件运算符
    //单目运算符  n++
    //双目运算符  a+b
    //三目运算符  布尔表达式？表达式1:表达式2
              //  （true到式1，false到式2）
    int M=4,N=8;
    int max;
    if(M>N) {max=M;
    }else {
    	max=N;
    }
    System.out.println("max="+max);
    //max=8
    max=M>N?M:N;
    System.out.println("max="+max);
    //max=8
   
    7.9
 java
       三大流程控制语句：顺序、选择（if else）、循环
   选择结构
         if(条件){语句；}    if(){}else{}
               多行注释  /*         */
               多重if结构:
                      if(表达式1)
                          {语句1;}
                        else if(表达式2)
                              {语句2;}
                           ...
                           else{语句n;}
               嵌套if结构
                      if(表达式1)
                      if（,,,）
                       语句；
                        else
                           语句；
         switch结构
              switch(表达式){
                    case 常量表达式1：
                          语句1；break;
                     case 常量表达式2：
                            语句2；break；
                       default:
                                  语句3；            
}
                     。。。.toUpperCase()//把字符串全部转化为。。。
   note :
               package imooc;
import java.util.Scanner;

public class a0709 {

	public static void main(String[] args) {
		
		
		/*System.out.println("请输出成绩；");
		Scanner sc=new Scanner(System.in);
		int score=sc.nextInt();
		if(score>=90) {System.out.println("优");}
		if(80<=score&score<90) {System.out.println("良");}
		if(60<=score&score<80) {System.out.println("中");}
		if(score<60) {System.out.println("不及格");}
		*/
		/*if(score>=90)
		{System.out.println("优");}
		else if(80<=score)//80<=score&score<90//score<=90不满足
		{System.out.println("良");}
		else if(60<=score)//60<=score&score<80
		{System.out.println("中");}
		else //else (score<60)
		{System.out.println("不及格");}
		*/
		  
		/*System.out.print("x=");
		Scanner sc=new Scanner(System.in);
		int x=sc.nextInt();
		if(x<0)
		{System.out.println("y=-1");}
		else if(x==0)
		{System.out.println("y=0");}
		else if(x>0)
		{System.out.println("y=1");}
		*/
		//x=-5
		//y=-1
		//int a=3,b=7;
		//if(a!=b) {
			//if(a<b) {System.out.println(a+"小于"+b);}
			//else {System.out.println(a+"大于"+b);}
		//}else {System.out.println(a+"等于"+b);}
		//3小于7
		
		Scanner sc=new Scanner(System.in);
		System.out.println("请输出1-7之间的数字");
		int n=sc.nextInt();
		  switch(n) {
		  case 1:System.out.println("星期一");break;
		  case 2:System.out.println("星期二");break;
		  case 3:System.out.println("星期三");break;
		  case 4:System.out.println("星期四");break;
		  case 5:System.out.println("星期五");break;
		  case 6:System.out.println("星期六");break;
		  case 7:System.out.println("星期天");break;
		  default:System.out.println("超出1-7");
		  请输出1-7之间的数字
                                   5
                                    星期五

		
		  }
		
		
	}

  7.10
循环：while循环，do-while循环，for循环，循环嵌套，break语句，continue语句
     while循环
                 while（循环条件）{语句；}
      do-while    
                  do{语句；}while（循环条件）；
                              Math.random()//[0,1)之间的数
       for循环
                   for（表达式1；表达式2；表达式3）
                          {语句}
                     package imooc;
import java.util.Scanner;
public class a0710 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
     /*int n=1;
     while(n<5){System.out.println(n);n++;}
     1
     2
     3
     4*/
     /*int sum=0;
     while(n<=5){sum=sum+n;n++;}
	System.out.println("sum="+sum);	
     sum=15*/
		 
     /*char eng='a';
     int c=1;
     while(eng<='z') {System.out.print(eng);eng++;if(c%13==0) {System.out.println();};c++;}
     abcdefghijklm
     nopqrstuvwxyz*/
	/*	int n=1,sum=0;
	do {
		sum=sum+n;n++;
	}while(n<=5);	
  System.out.println(sum);
  15*/
		/*int number=5;
		int guess;
		System.out.println("请输入1-10之间的数");
		do {System.out.println("你猜的数为：");
		Scanner sc=new Scanner(System.in);
	    guess=sc.nextInt();
		if(guess<number) {System.out.println("太小");};
		if(guess>number) {System.out.println("太大");};
		
		
		}while(number!=guess);
		System.out.println("恭喜你猜对了");
请输入1-10之间的数
你猜的数为：
2
太小
你猜的数为：
6
太大
你猜的数为：
9
太大
你猜的数为：
5
恭喜你猜对了*/
		
		/*int number=(int)(Math.random()*10+1);//强制类型转换 double转化为int 
		int guess;
		System.out.println("请输入1-10之间的数");
		do {System.out.println("你猜的数为：");
		Scanner sc=new Scanner(System.in);
	    guess=sc.nextInt();
		if(guess<number) {System.out.println("太小");};
		if(guess>number) {System.out.println("太大");};
		
		
		}while(number!=guess);
		System.out.println("恭喜你猜对了");
		请输入1-10之间的数
		你猜的数为：
		5
		太小
		你猜的数为：
		4
		太小
		你猜的数为：
		6
		太小
		你猜的数为：
		7
		太小
		你猜的数为：
		8
		恭喜你猜对了*/
		
		7.13
 for循环
    for（表达式1；表达式2；表达式3）{语句；}
        例：for（int n=1；n<5;n++）{}//变量n只有在{}中有用
                  执行顺序   for(1;2;4){3}
                    break 跳出循环//if(...)break
           package imooc;

public class a0713 {
	public static void main(String[] args) {
		int sum=0;
		for(int n=1;n<=5;n++) {sum=sum+n;}
		System.out.println("sum="+sum);
		sum=15 
   



