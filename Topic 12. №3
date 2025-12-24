#include <iostream>
#include <fstream>
#include <string>
#include <cctype>
#include <bitset>
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
    
    string line;
    getline(in, line);
    string result;
    string num_str;
    
    for (char c : line) {
        if (isdigit(c)) {
            num_str += c;
        } else {
            if (!num_str.empty()) {
                int num = stoi(num_str);
                result += bitset<32>(num).to_string().substr(bitset<32>(num).to_string().find('1'));
                num_str.clear();
            }
            result += c;
        }
    }
    
    if (!num_str.empty()) {
        int num = stoi(num_str);
        result += bitset<32>(num).to_string().substr(bitset<32>(num).to_string().find('1'));
    }
    
    out << result;
    in.close();
    out.close();
    
    return 0;
}
