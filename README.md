# atm_bank
#include<iostream.h>
#include<stdio.h>
class customer{
	public:
	int bal;
	string name;
	long acc;
	void enter()
	{
		cout<<"------:::::Enter the detail of customer:::::------"<<endl;
		cout<<"Enter Name of customer"<<endl;
		cin>>name;
		cout<<"Enter Account number of customer"<<endl;
		cin>>acc;
		cout<<"Enter Bank balance of customer"<<endl;
		cin>>bal;
		
		}
	void display();
	};
	void customer:: display()
	{
		
	//	goto(30,40);
		cout<<" Detail of customer is:-"<<endl;
		cout<<" Name of customer is:-"<<name<<endl;
		
		cout<<" Account number of customer is:-"<<acc<<endl;
		
		cout<<" Bank balance of customer is:-"<<bal<<endl;
		
			if(bal<100)
			
	cout<<"detail ofcustomer bank balance less then 100 is:-"<<endl<<name<<endl<<acc<<endl<<bal<<endl;
			else
			cout<<"now balance is greater then 100"<<endl;
		
		}
	class banker:public customer
	{
		public:
		void bank()
		{
			long pass;
		long  naas=123456789;
		cout<<":::===welcome to atm room===:::"<<endl;
		cout<<"Enter your ATM password"<<endl;
		cin>>pass;
		if (pass==naas)
		
		{
		cout<<"Your password is right";
		      
		}
		else
		
			cout<<"your password is worng"<<endl;
		}
		};
		int main()
		{ int i,n;
		long h,p=123456789;
		cout<<"Enter your  password "<<endl;
		cin>>h;
		if(h==p){
		cout<<"Enter number of customer"<<endl;
		      cin>>n;
		      customer c[n];
		   for(i=1;i<=n;i++)
		   {
			
			c[i].enter();
			c[i].display();
			cout<<"now we are in object "<<i<<endl;
		   }
		   banker k;
		   k.bank();
			
		}
		else
		cout<<"baba g ka thulu";
		}
