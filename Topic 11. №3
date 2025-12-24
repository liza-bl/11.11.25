#include <iostream>
#include <list>
#include <string>
using namespace std;

int main() {
    list<string> students = {"Иванов", "Петров", "Сидоров", "Алексеев", "Борисов"};
    students.sort();
    students.remove_if([](const string& surname) {
        return !surname.empty() && surname[0] == 'А';
    });
    for (const auto& student : students) {
        cout << student << endl;
    }
    
    return 0;
}
