# oop-functions
#include <iostream>
using namespace std;

class Car {
private:
    string brand;
    int year;

public:
    Car(string b, int y) : brand(b), year(y) {}

    void setBrand(string b) { brand = b; }
    string getBrand() { return brand; }
    int getYear() { return year; }

    void displayInfo() {
        cout << "Car Brand: " << brand << endl;
        cout << "Manufacturing Year: " << year << endl;
    }
};

int main() {
    Car myCar("Toyota", 2015);
    myCar.displayInfo();

    myCar.setBrand("Honda");
    cout << "\nUpdated Car Details:" << endl;
    myCar.displayInfo();

    return 0;
}

