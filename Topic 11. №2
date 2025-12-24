#include <iostream>
#include <deque>
#include <string>
using namespace std;

int main() {
    deque<string> orders;
    orders.push_back("Order1");
    orders.push_back("Order2");
    orders.push_back("Order3");
    orders.push_front("UrgentOrder1");
    orders.push_front("UrgentOrder2");
    orders.pop_front();
    orders.pop_front();
    
    for (const auto& order : orders) {
        cout << order << endl;
    }
    
    return 0;
}
