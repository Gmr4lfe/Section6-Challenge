#include <iostream>

using namespace std;

int main() {
    
    cout<< "Hello, welcome to Frank's Carpet Cleaning Service"<< endl;
    cout<< "How many small room do you need cleaned?: ";
    
    int number_of_small_rooms {0};
    cin >> number_of_small_rooms;
    
    int number_of_large_rooms {0};
    cout << "How many large rooms do you need cleaned?: ";
    cin >> number_of_large_rooms;
    
    const double price_per_small_room {25.0};
    const double price_per_large_room {35.0};
    
    const double sales_tax {0.06};
    const double estimate_expiration {30}; // days
    
    cout <<"\nEstimate for carpet cleaning service" << endl;
    cout << "Number of small rooms: "<< number_of_small_rooms<< endl;
    cout << "Number of large rooms: " << number_of_large_rooms<< endl;
    cout << "Price per small room: $"<< price_per_small_room << endl;
    cout << "Price per large room: $"<< price_per_large_room << endl;
    cout << "Cost: $"<<(price_per_small_room * number_of_small_rooms) + (price_per_large_room*number_of_large_rooms) <<endl;
    cout <<"Tax: $"<< ((price_per_small_room * number_of_small_rooms + price_per_large_room* number_of_large_rooms)*sales_tax) << endl;
    cout<< "========================================"<< endl;
    
    
    cout<< "Total estimate: $"<< ((price_per_small_room*number_of_small_rooms + price_per_large_room* number_of_large_rooms)*sales_tax) + (price_per_small_room*number_of_small_rooms) + (price_per_large_room*number_of_large_rooms)<< endl;
    
    cout<< "This estimate is valid for "<< estimate_expiration <<" days."<< endl;
    
    cout << endl;
    
    return 0;
    
}
