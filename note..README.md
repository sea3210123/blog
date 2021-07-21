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
   7.14
嵌套
      while嵌套
                    while（）{while(){}}
   求1!+2!+3!....10!=
              /*	int n=1,m=1,h=1,j=0;
		while(h<=10) {while(n<=h) {m=m*n;n++;}
	h++;j=j+m;	}
		System.out.println(j);
	}
	//4037913*/
		/*int j=0;//必须在循环外面
		for(int n=1,m=1;m<=10;m++) 
		{n=1;
			for(int h=1;h<=m;h++)
		{n=n*h;};
		j=n+j;}
		System.out.println(j);
		//4037913*/
         continue语句  跳出本次循环，继续下次循环
                          if()continue
  程序调试 --debug
         1 断点
          2单步调试F5
       F8 从一个断点跳到另一个断点
.16
  声明数组   int[] m;
  创建数组  m=new int[9];
                int[] m=new int[9];
  初始化    int[] m={'a'};
package imooc;
import java.util.Scanner;
import java.util.scanner;
public class a0716 {
	public static void main(String[] args) {
		/*//求数组累加和
		int[] a=new int[5];
		Scanner sc=new Scanner(System.in);
	  
		for(int i=0;i<a.length;i++) {
			 System.out.println("请输出第"+(i+1)+"数字");
			 a[i]=sc.nextInt();
		}
		System.out.print("你输入的数组为:");
		for(int i=0;i<a.length;i++) {
			System.out.print(a[i]+" ");
		}
		int sum=0;
		for(int i=0;i<a.length;i++) {
			sum=sum+a[i];
		}
		System.out.println();
		System.out.println("你的数组和为"+sum);
   //请输出第1数字
	5
	请输出第2数字
	6
	请输出第3数字
	8
	请输出第4数字
	66
	请输出第5数字
	5
	你输入的数组为:5 6 8 66 5 
	你的数组和为90
    */
// 求数组中最大值
		int[] a= {908,6758654,896,978};
		int max=a[1];
		for(int n=0;n<a.length;n++) {
		if(max<a[n]) {
		max=a[n];
		}
		}
		System.out.println("max"+"="+max);
//max=6758654
 7.21
  无参无返回值方法
            public class a0721 {
	public void star() {
		System.out.println("*********");
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
       a0721 a=new a0721();
       a.star();
	}

}
   无参带返回值方法
                public int a(){}
        public int area(){
   	   int length=7;
   	   int width=8;
   	   int s=length*width;
   	   return s;
      }
         // 无参带返回值方法
     a0721 S=new a0721();
     System.out.println("S="+S.area())
;

   带参无返回值
          public void a(float a,float b){}
       // public void max(float a,float b) {
		 float max;
		   if(a<b) {
			   max=b;
		   }else {
			   max=a;
		   }
		   System.out.println("max="+max);
		    
	   }
        /*  a0721 bc=new a0721();
     float a=4f,b=7f;
     bc.max(a, b);
     bc.max(34f, 67f);
    // max=7.0
     max=67.0*/
有参有返回值的方法 (方法不能嵌套定义)
      public int fac(int n){}
//求1！+2！+3！+4！+5！=
            public int jc(int n) {
		 int s=1;
		 for(int i=1;i<=n;i++) {
			 s*=i;
		 }
		 return s;
	 }
              a0721 a=new a0721();
        
         System.out.println("3!="+a.jc(3));
         int sum=0;
        for(int i=1;i<=5;i++) {
        	sum+=a.jc(i);
        }
       System.out.println("sum="+sum);
      //数组做参数
    public void sz(int[] arr) {
		for(int i=0;i<arr.length;i++) {
			System.out.print(arr[i]+" ");
		}
	}   
int[] n= {34,2,11,22};
       a.sz(n);
//34 2 11 22 
 
//数组中找数字
         public void sz(int[] arr) {
		for(int i=0;i<arr.length;i++) {
			System.out.print(arr[i]+" ");
		}
	}
	 public boolean search(int n,int[]arr) {
		 boolean a1=false;
		 for(int i=0;i<arr.length;i++) {
			 if(arr[i]==n) {
				a1=true;
				break;
			 }
		 }
		 return a1;
	 }
               /*a0721 a=new a0721();
	 * 	int[] m= {34,23,55,67,43,12};
		System.out.println("请输入你要找的数字");
		Scanner sc=new Scanner(System.in);
		int e=sc.nextInt();
		
		if(a.search(e, m)==true) {
			System.out.println("找到了");
		}else {
			System.out.println("没找到");
		}
	//	请输入你要找的数字
		54
		没找到*/
         方法重载  方法名相同参数不同
                       public int pluse(int m,int n) {
		return m+n;
	}
	public double pluse(double m,double n) {
		return m+n;
	}
	public int pluse(int[] arr) {
		int sum=0;
		for(int i=0;i<arr.length;i++) {
			sum+=arr[i];
		}
		return sum;
	}
                   /* int[] a1= {23,4,56,77,88,87};
		 a0721 a=new a0721();
		  int n=8,m=7;
		  double aa=6.7,b=5.8;
		 System.out.println("sum="+a.pluse(a1));
		 System.out.println("m+n="+a.pluse(m, n));
		 System.out.println("aa+b="+a.pluse(aa, b));
		// sum=335
				 m+n=15
				 aa+b=12.5

		*/ 



