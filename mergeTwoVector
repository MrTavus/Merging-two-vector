#include <iostream>
#include <vector>
using namespace std;

vector<int> merge(vector<int>&, vector<int>&);

int main(){

	vector<int> v1;
	vector<int> v2;
	v1.push_back(1);
	v1.push_back(3);
	v1.push_back(4);
	v1.push_back(8);
	v1.push_back(10);
	v1.push_back(15);
	v2.push_back(2);
	v2.push_back(3);
	v2.push_back(4);
	v2.push_back(5);
	v2.push_back(11);
	v2.push_back(15);
	v2.push_back(16);
	v2.push_back(20);

	vector<int> merged = merge(v1,v2);
	
	for(int i =0;merged[i];i++){
		cout << merged[i] << " ";
	}
	cout << endl;
}

vector<int> merge(vector<int>& v1, vector<int>& v2){
	vector<int> mergeVector;
	
	int i=0,j=0;

	while(i<v1.size() && j<v2.size()){
		if(v1[i] == v2[j]){
			mergeVector.push_back(v1[i]);
			mergeVector.push_back(v2[i]);
			i++;
			j++;		
		}
		else if(v1[i] < v2[j]){
			mergeVector.push_back(v1[i]);
			i++;
		}
		else{
			mergeVector.push_back(v2[i]);
			j++;
		}
	}

	while(i!=v1.size()){
		mergeVector.push_back(v1[i]);
		i++;
	}
	while(j!=v2.size()){
		mergeVector.push_back(v2[j]);
		j++;
	}
	return mergeVector;
}
