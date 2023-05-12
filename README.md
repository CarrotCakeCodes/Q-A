# Q-A
Actually this is not a real project, i just want to ask a question but don't know where to push it :D
honestly speeking i am not sure that sb will read this as the preceding trials...

one of Codeforces problems i solved it but it gives me time limit exceeded at test case 22, if you can help i will be very thankful 
https://codeforces.com/contest/299/problem/A

#include <iostream>

using namespace std;

int main()

{

     const int max_capacity= 10e5;

     int arr[max_capacity];

     int flag=0;

     int actual_size;

     cin>> actual_size;

     for(int i=0; i<actual_size; i++)

        cin>> arr[i];

     for(int n=0; n<actual_size; n++)   

     //n=denomenator & j= numenerator

     {

         for (int j=0; j<actual_size; j++)

         {

            if(arr[j]<arr[n])

            {  flag=0;

                break;

            }
                       
           if( arr[j]% arr[n]==0)

                flag=1;

             else

             {

                 flag=0;

                 break;

             }

         }

         if(flag)

         {

            cout<< arr[n];

            return 0;

         }

     }

     if(flag==0)

        cout<< -1;       

}

https://codeforces.com/submissions/nourhan-mohsen
 those are all my trials, you may have a look                
