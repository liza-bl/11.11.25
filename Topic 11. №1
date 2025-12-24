#include <iostream>
#include <array>
#include <numeric>
#include <iomanip>
using namespace std;

int main() {
    array<int, 10> arr;
    for (size_t i = 0; i < arr.size(); ++i) {
        arr[i] = i + 1;
    }
    double average = static_cast<double>(accumulate(arr.begin(), arr.end(), 0)) / arr.size();
    cout << fixed <<setprecision(2) << average << endl;
    
    return 0;
}
