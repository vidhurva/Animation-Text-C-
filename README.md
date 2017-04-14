# Animation-Text-C-
Animation in C++ Using Loops

 #include <iostream>
 #include <stdlib.h>
 using namespace std;
 
 void text_animation(char a[100])
 {
         int i;
         double k;
 
         for(i=0;a[i]!='\0';i++)
         {
            for(k=0;k<30000000;k++);
            cout<<a[i];
         }
 }
  
 //call by reference 
 void slide_animation(char *a)
 {
         int i, k;
         double j;

// screen width

            for(k=0;k<70;k++)
         {
            for(i=0;i<k;i++)
         {
            cout << "  ";
         }
         cout << a;
 
 // wait time for text
 
            for(j=0;j<1000000;j++);
            system("cls");
}
          cout<<"                    "<< a <<"                               ";
 }
 int main()
 {
         slide_animation(" Hello Humans! ");
         return 0;
}
