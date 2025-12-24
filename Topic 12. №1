#include <iostream>
#include <fstream>
#include <string>
#include <algorithm>
#include <cctype>
using namespace std;

int main() {
    ifstream in;
    ofstream out;
    in.open("input.txt");
    out.open("output.txt");
    
    if (!in.is_open() || !out.is_open()) {
        cerr << "Unable to open file!" << endl;
        return 1;
    }
    
    string text;
    getline(in, text);
    string remove_chars = "useragreement";
    
    text.erase(remove_if(text.begin(), text.end(), [&](char c) {
        return remove_chars.find(tolower(c)) != string::npos;
    }), text.end());
    
    out << text;
    in.close();
    out.close();
    
    return 0;
}
```
