---
id: isuZbpDxnkAPr9IPuFIfz
title: C++ Const
desc: ''
updated: 1639771141678
created: 1639771140562
---

## `const` with functions

Reference: [Video](https://www.youtube.com/watch?v=RC7uE_wl1Uc&ab_channel=BoQian)

Using const in methods examples, and can be used for more efficiency.

```cpp

class Dog {
    // Class Memebers
    int age;
    string name;

    public:
    Dog() {age =3; name = "dummy";}
    
    // Const parameter
    void setAge (const int& a ) {age = a;} // Correct[ pass by reference and can't be changed]
    void setAge (const int a ) {age = a;} // const is not useful here
    void setAge (int a ) {age = a;} // similar

    //  Const return value
    const string& getName() {return name;}; // pass by reference "more efficient"

    //const function [Means it will not modify any members of the class]
    void printDogName() const {
        cout << getName() << "const" << endl; // const functions can only called const functions
    }
    // Overload const function (will be called if instance of the class is const)
    void printDogName() {
        cout << name << "non-const" << endl; // const functions can only called const functions
    } 
     
}

int main(){
    // Call regular
    Dog d;
    d.printDogName();

    // Call overloaded 
    const Dog d2;
    d2.printDogName();
    }


```



