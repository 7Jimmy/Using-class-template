# Using-class-template
#include<iostream>
using namespace std;
template <class T>
class test{
	private:
		T arr[3];
		public:
			void in(){
				for(int i=1;i<=3;i++){
					cin>>arr[i];
				}
			}
			void out(){
				for(int i=1;i<=3;i++){
					cout<<arr[i]<<endl;
				}
			}
};
int main(){
	test<int>x;
	x.in();
	x.out();
	test<char>y;
	y.in();
	y.out();
	return 0;
}
