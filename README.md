# brmrush.github.io

```cpp
#include <iostream>

using namespace std;

class ICar {
    //Pure virtual function to declare this class as an abstract class
    virtual void drive() = 0;
}

class Audi : public ICar {
    void drive () override
    {
        cout << "I'm driving an Audi\n";
    }
}

class Mercedes : public ICar {
    void drive () override
    {
        cout << "I'm driving a Mercedes\n";
    }
}


int main()
{
    ICar *ptrAudi = new Audi;
    //Calls drive function of Audi class
    ptrAudi->drive();
}

```
