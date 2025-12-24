#include <iostream>
#include <fstream>
#include <string>
using namespace std;

int main() {
    ifstream in1;
    ifstream in2;
    ofstream out;
    in1.open("input1.txt");
    in2.open("input2.txt");
    out.open("output.txt");
    
    if (!in1.is_open() || !in2.is_open() || !out.is_open()) {
        cerr << "Unable to open file!" << endl;
        return 1;
    }
    
    string X, Y;
    getline(in1, X);
    getline(in2, Y);
    
    if (X.find(Y) != string::npos) {
        out << "yes";
    } else {
        out << "no";
    }
    
    in1.close();
    in2.close();
    out.close();
    
    return 0;
}
