#include<iostream>
#include<string>
#include<fstream>
using namespace std;
int main()
{
    string name,yesno,repeatMain;
	int quantity,type,bname,cname,pname,current= 0,totalamt= 0,B1=200,B2=250,B3=222,B4=150,B5=235,P1=350,P2=300,P3=230,P4=229,P5=199,C1=150,C2=99,C3=149,C4=199,C5=160;
	ofstream mywritefile("dish.txt");

    cout<<"\t\t                                          WELCOME                                                    "<<endl;
    cout<<"\n";	
    cout<<"\t\t%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%"<<endl;
    cout<<"\t\t%                                        MENU CARD                                               %"<<endl;
    cout<<"\t\t%                                                                                                %"<<endl;
    cout<<"\t\t%   1.BURGERS                      2.PIZZAS                         3.CHINESE                    %"<<endl;
    cout<<"\t\t%                                                                                                %"<<endl;
    cout<<"\t\t%   1.VEGGIE BURGER     200 RS. | 6 .MARGHERITA PIZZA   350 RS.  | 11.KUNG PAO CHICKEN  150 RS.  %"<<endl;
    cout<<"\t\t%   2.CHEESE BURGER     250 RS. | 7 .PEPPERONINI PIZZA  300 RS.  | 12.HOT POT            99 RS.  %"<<endl;
    cout<<"\t\t%   3.TURKEY BURGER     222 RS. | 8 .HAWAIIAN PIZZA     230 RS.  | 13.DIM SUM           149 RS.  %"<<endl;
    cout<<"\t\t%   4.BLACK BEAN BURGER 150 RS. | 9 .MEAT PIZZA         229 RS.  | 14.DUMPLINGS         199 RS.  %"<<endl;
    cout<<"\t\t%   5.KIMCHI BURGER     235 RS. | 10.CHICAGO PIZZA      199 RS.  | 15.XIAOLONGBAO       160 RS.  %"<<endl;
    cout<<"\t\t%                                                                                                %"<<endl;
    cout<<"\t\t%                                                                                                %"<<endl;
    cout<<"\t\t%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%"<<endl;
    cout<<"\n";
    cout<<"\n\t\t\t PLEASE ENTER YOUR NAME: ";
    cin>>name;
    mywritefile<<"CUSTOMER NAME:"<<name<<endl;
    cout<<"\n";

    do{
    cout<<"\t\t\t PLEASE SELECT YOUR DISH TYPE: ";
    cin>>type;
   // burger
    if (type==1) {
    cout<<"\n\t\t\t PLEASE ENTER YOUR DISH NAME:";
    cin>>bname;
    cout<<"\n";
    if (bname==1) {
    cout<<"\t\t\t YOU HAVE SELECTED VEGGIE BURGER."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED VEGGIE BURGER. QUANTITY:";
        
    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
            cout<<"\n";
    mywritefile<<quantity<<"\n";
        cout<<"\n";

    current= B1*quantity;
    } 
    else if(bname==2) {
    cout<<"\t\t\t YOU HAVE SELECTED CHEESE BURGER."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED CHEESE BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT: ";
    cin>>quantity;
            cout<<"\n";

        mywritefile<<quantity<<"\n";

    current=B2*quantity;
    } 
    else if(bname==3) {
    cout<<"\t\t\t YOU HAVE SELECTED TURKEY BURGER."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED TURKEY BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";

    cin>>quantity;
            cout<<"\n";
        mywritefile<<quantity<<"\n";
    current=B3*quantity;
    } 
    else if(bname==4) {
    cout<<"\t\t\t YOU HAVE SELECTED BLACK BEAN BURGER."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED BALCK BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
        cout<<"\n";
        mywritefile<<quantity<<"\n";

    current = B4 * quantity;
    } 
    else if(bname==5){
    cout<<"\t\t\t YOU HAVE SELECTED KIMCHI BURGER."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED KIMCHI BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
        cout<<"\n";
        mywritefile<<quantity<<"\n";
    current= B5*quantity;
    }
	} 
    // Pizza
    else if(type==2){
    cout<<"\n\t\t\t PLEASE ENTER YOUR DISH NAME:";
    cin>>pname;
    cout<<"\n";
    if(pname==6){
    cout<<"\t\t\t YOU HAVE SELECTED MARGHERITA PIZZA."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED MARGHERITA BURGER. QUANTITY:";
    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT: ";
    cin>>quantity;
            cout<<"\n";
        mywritefile<<quantity<<"\n";
    current=P1 *quantity;
 }
  else if (pname== 7) {
    cout<<"\t\t\t YOU HAVE SELECTED PEPPERONINI PIZZA."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED PEPPERONINI BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
        cout<<"\n";
    mywritefile<<quantity<<"\n";

    current=P2*quantity;
   }
    else if(pname==8) {
    cout<<"\t\t\t YOU HAVE SELECTED HAWAIIAN PIZZA."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED HAWAIIAN BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
        cout<<"\n";
            mywritefile<<quantity<<"\n";


    current=P3*quantity;
    } 
    else if(pname==9) 
	{
    	
    cout<<"\t\t\t YOU HAVE SELECTED MEAT PIZZA."<<endl;
        cout<<"\n";
                mywritefile<<"CUSTOMER ORDERED MEAT BURGER. QUANTITY:";
    cout<<"\t\t\t ENTER HOW MANY QUNTITY YOU WANT:";
        cout<<"\n";
    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current=P4*quantity;
    } 
    else if(pname==10) {
    cout<<"\t\t\t YOU HAVE SELECTED CHICAGO PIZZA."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED CHICAGO BURGER. QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
        
        cout<<"\n";

    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current=P5*quantity;
    }
    } 
        //chinese
    else if(type==3)
	 {
    cout<<"\n\t\t\t PLEASE ENTER YOUR DISH NAME:";
    cin>>cname;
    cout<<"\n";
    if(cname==11){
    cout<<"\t\t\t YOU HAVE SELECTED KUNG PAO CHICKEN."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED KUNG PAO CHICKEN . QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";
    cin>>quantity;
            mywritefile<<quantity<<"\n";

    current=C1*quantity;
    } 
    else if(cname==12){
    cout<<"\t\t\t YOU HAVE SELECTED HOT POT."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED HOT POT . QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT: ";
        cout<<"\n";

    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current=C2*quantity;
    } 
    else if(cname==13) {
    cout<<"\t\t\t YOU HAVE SELECTED DIM SUM."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED DIM SUM . QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT: ";

    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current=C3*quantity;
    } 
  else if(cname==14){
    cout<<"\t\t\t YOU HAVE SELECTED DUMPLINGS."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED DUMPLINGS . QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT: ";

    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current= C4*quantity;
    } 
   else if(cname==15) {
    cout<<"\t\t\t YOU HAVE SELECTED XIAOLONGBAO."<<endl;
        cout<<"\n";
        mywritefile<<"CUSTOMER ORDERED XIAOLONBAO . QUANTITY:";

    cout<<"\t\t\t ENTER HOW MANY QUANTITY YOU WANT:";

    cin>>quantity;
                mywritefile<<quantity<<"\n";

    current=C5*quantity;
    }
    }

totalamt += current; 
cout<<"\t\t\t Do you want to order anything else? (yes/no):";
cin>>repeatMain;
cout<<"\n";

    } while(repeatMain== "yes");
do{
    cout<<"\t\t\t THANK YOU FOR ORDERING "<< name <<" SIR. YOUR TOTAL BILL IS: "<<totalamt<<" Rs."<<endl;
    mywritefile<<"CUSTOMER TOTAL BILL IS "<<totalamt<<endl;
    break;
}while(repeatMain == "no");
mywritefile.close();
	string mytext;
	ifstream myreadfile("filename.txt");
	while(getline(myreadfile,mytext));{
		cout<<mytext;
}
return 0;
}
# food-ordering-system
Developed food ordering system for automating restaurant order taking and bill generation
