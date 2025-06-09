If statements
```cpp
#include <iostream>

int main() {
  // Write code here
  int level =1; 

  if (level >21) {
    std::cout <<"💎 Diamond: Level 21 -25\n";
  }
  else if (level> 15){
    std::cout << "🏅 Platinum: Level 16-20\n";
  }
  else if (level >10){
    std::cout<< "🥇 Gold: Level 11-15\n";
  }
  else if (level >5){
    std::cout<< "🥈 Silver: Level 6-10\n";
  }
  else {
    std::cout<<"🥉 Bronze: Level 1-5\n";
  }
}
```
Fortune Cookie Random Numbers
```cpp
#include <iostream>
#include <cstdlib>

int main(){
  srand(time(NULL));
  int fortune = std::rand() % 6;  // Generates a random number that's either 0, 1, 2, 3, 4, 5

  if(fortune == 0){
     std::cout << "Don't pursue happiness – create it.\n";
  } 
  else if (fortune == 1) {
    std::cout << "All things are difficult before they are easy.\n";
  }
  else if (fortune == 2) {
    std::cout << "Someone in your life needs a letter from you.\n";
  }
  else if (fortune == 3) {
    std::cout << "The fortune you search for is in another cookie.\n";
  }
  else if (fortune == 4) {
    std::cout << "Help! I'm being held prisoner in a Chinese bakery!\n";
  }
  else if (fortune == 5) {
    std::cout << "The early bird gets the worm, but the second mouse gets the cheese.\n";
  }

int num1 = std::rand() % 50;
int num2 = std::rand() % 50;
int num3 = std::rand() % 50;
int num4 = std::rand() % 50;
int num5 = std::rand() % 50;
int num6 = std::rand() % 50;

std::cout <<"Lucky number: " <<num1<<" "<<num2<<" "<<num3<<" "<<num4<<" "<<num5<<" "<<num6;
}
```
AND OR NOT operators 
```cpp
#include <iostream>

int main() {
  // Write code here
  int age = 200;
  bool citizen = false; 
  bool registered = true;
  if (age>17 and citizen and registered){
    std::cout <<"You can vote!\n";
  } 
  else if (age<18){
    std::cout<<"You are not old enough to vote.\n";
  }
  else if(citizen==false){
    std::cout<<"You are not eligible to vote\n";
  }
  else if(registered==false){
    std::cout<<"You need to register first.\n";
  }
  else {
    std::cout<<"You have not met the requirements unfortantely.";
  }
}
```
Trivia Quiz Game 
```cpp
#include <iostream>

  

int main() {

  // Write code here

  std::cout << "==================\n";

  std::cout << "Welcome to Trivia!\n";

  std::cout << "==================\n";

  int answer1;

  int answer2;

  std::string answer3;

  int count=0;

  std::cout<<"Q1) What is the name of the world's longest river? 💧\n";

  std::cout<<"1) Missouri River\n";

  std::cout<<"2) Nile\n";

  std::cout<<"3) Amazon River\n";

  std::cout<<"4) Yangtze River\n";

  std::cin >> answer1;

  

  if (answer1 == 2){

    std::cout<<"You are right!\n";

    count+=1;

  }

  else {

    std::cout<<"im sorry...\n";

  }

  std::cout<<"Q2) How many bones are in the human body? 🦴\n";

  std::cout<<"1) 92\n";

  std::cout<<"2) 150\n";

  std::cout<<"3) 206\n";

  std::cout<<"4) 10 \n";

  std::cin >> answer2;

  if (answer2 == 3){

    std::cout<<"You are right!\n";

    count+=1;

  }

  else {

    std::cout<<"im sorry...\n";

  }

  std::cout<<"Q3) What food never spoils? 😷\n ";

  std::cout<<"please type your anwser: ";

  std::cin >> answer3;

  

  if(answer3 == "Honey" or answer3 == "honey"){

    std::cout<<"You are right!\n";

    count+=1;  

  }

  else {

    std::cout<<"im sorry...\n";

  }

  std::cout<<"The total amount of right Trivia questions: " << count;

}
```
While loops
```cpp
#include <iostream>

int main() {
  // guess a number
  int answer; 
  while (answer !=64){
    std::cout <<"Guess the number: ";
    std::cin >> answer; 
  }

  if(answer==64){
    std::cout <<"You guess right, it was 64!";
  }
}
```
For loops
```cpp
#include <iostream>

int main() {
  // Write code here
  for (int i=0; i<51; i++) {
    std::cout<<i<<" sheep\n";
  }
  std::cout<<"😴💭";
}
```
```
#include <iostream>

int main() {
  // Write code here
  for (int i=99; i>0; i--){
    std::cout<<i <<" bottles of beer on the wall\n";
    std::cout<<i <<" bottles of beer\n";
    std::cout<<"Take one down, pass it around\n";
    std::cout << i-1 << " bottles of beer on the wall\n\n";
  } 
```
[Fizz Buzz](https://en.wikipedia.org/wiki/Fizz_buzz)
```cpp
#include <iostream>

int main() {

  // Write code here

  for(int i = 1; i <51; i++) {

    if(i % 3 == 0 & i % 5 ==0){

      std::cout<<"FizzBuzz\n";

    }

    else if(i%3 ==0){

      std::cout<<"Fizz\n";

    }

    else if(i%5==0){

      std::cout<<"Buzz\n";

    }

    else{

      std::cout<<i<<"\n";

    }

  }

}
```
Vectors
```cpp
#include <iostream>

#include <vector>

int main() {

  // Write code here 💖

  std::vector<int> Item = {1,2,3,4,5,6,7,8,9,10};

  std::vector<std::string> gears = {"hello","hello2"};

}


#include <iostream>

#include <vector>

int main() {

  // Write code here 💖

  std::vector<int> lemonade = {25,28,40,85,76};

  std::vector<double> sales = {75.50,89.25,60.00,102.45, 95.10};

  std::cout<<lemonade[4] << "\n";

  std::cout<<sales[4] << "\n";

  std::cout<<lemonade[4]/sales[4] <<"\n";

}

#include <iostream>

#include <vector>

int main() {

  // Write code here 💖

  std::vector<std::string> cart ={"🍕 Pepperoni pizza","🥗 Garden salad","🥤 Diet Coke"};

  cart.push_back("🥫 Marinara sauce");

   for (int i = 0; i < cart.size(); i++) {

     std::cout << cart[i] << " ";

  }

  std::cout<<cart.size();

  std::cout<<"\n";

  cart.pop_back();

   for (int i = 0; i < cart.size(); i++) {

     std::cout << cart[i] << " ";

  }

  std::cout<<cart.size();

}
```
Sum of Even / Product of Odd
```cpp
#include <iostream>

#include <vector>

  

int main() {

  int Even = 0;

  int Odd = 1;

  // Write code here 💖

  std::vector<int> num = {2,4,3,6,1,9,8,0,8,5,7,3,3};

  for(int i=0; i<num.size(); i++){

    if(num[i]%2==0){

      Even=Even+num[i];

    }

    else {

      Odd=Odd*num[i];

    }

  }

  std::cout<<Even<<"\n";

  std::cout<<Odd<<"\n";

}
```
Declaring Function
```cpp
void name () {}

#include <iostream>

#include <vector>

void welcome(){

  std::cout << "1. 🍔 Cheeseburger\n";

  std::cout << "2. 🍟 Fries\n";

  std::cout << "3. 🥤 Soda\n";

  std::cout << "4. 🍦 Ice Cream\n";

  std::cout << "5. 🍪 Cookie\n";

  }

  

int main() {

  // Write code here 💖

  welcome();

  welcome();

}

#include <iostream>

void ooo_message(std::string date){

  std::cout<<"Thank you for your email.\n";

  std::cout<<"I am currently out of the office and will be back "<<date<<".\n";

  std::cout<<"I will respond as soon as I can upon my return.\n";

}

int main() {

  // Write code here

  ooo_message("10/20/2025");

}

// Conversions ➡️

// Codédex

  

#include <iostream>

  

int temp_conversion(int number) {

  int result = 0;

  result = (number - 32) * 5/9;

  return result;

}

  

int main() {

  std::cout<<temp_conversion(100);

}
```
- The _parameter_ is the variable listed inside the parentheses in the function definition (when we define the function).
- The _argument_ is the value sent to the function (when we call the function).
Tips Calculator
```cpp
#include <iostream>

void tips_menu(){

  int answer = 0;

  std::cout<<"Leave a Tip? \n";

  std::cout<<"15%   20%   %25 \n";

  std::cout<<"   custom    \n";

}

  

float tips_calculator(float percentage, float cost){

  float result = 0;

  result = cost + ((percentage/100) * cost);

  return result;

}

  

float shared_bills(float percentage, float cost, int number){

  float result = 0;

  result = (cost + ((percentage/100) * cost))/number;

  return result;

}

  

float shared_bills_new(int number, float tips){

  float result = 0;

  result = tips/number;

  return result;

}

  

int main() {

  // Write code here

  tips_menu();

  std::cout<<tips_calculator(20,50)<<"\n";

  std::cout<<shared_bills(20,50,2)<<"\n";

  std::cout<<shared_bills_new(2,tips_calculator(20,50));

}
```
classes and objects in C++
```cpp

class Car {
  public:
    // Attributes
    std::string brand;
    std::string model;
    int year;
    
    // Method
    void honk() {
      std::cout << "Beeep! 🚗" << std::endl;
    }
};


int main() {
  // Creating an object of Car
  Car myCar;
  
  // Accessing the attributes and setting their values
  myCar.brand = "Toyota";
  myCar.model = "Corolla";
  myCar.year = 2021;
  
  // Calling a method
  myCar.honk();

  // Outputting the attributes
  std::cout << "My car is a " << myCar.year << " " 
            << myCar.brand << " " << myCar.model << "." << std::endl;

  return 0;
}
```
Constructors
```cpp
#include <iostream>
#include <string>

class Car {
public:
    std::string brand;
    int year;
    
    // Default constructor
    Car() : brand("Unknown"), year(0) {
        std::cout << "Default constructor called.\n";
    }

    // Parameterized constructor
    Car(std::string b, int y) : brand(b), year(y) {
        std::cout << "Parameterized constructor called.\n";
    }

    // Copy constructor
    Car(const Car &c) : brand(c.brand), year(c.year) {
        std::cout << "Copy constructor called.\n";
    }
};

int main() {
    // Using the default constructor
    Car car1;
    std::cout << "Car 1: " << car1.brand << ", " << car1.year << "\n";

    // Using the parameterized constructor
    Car car2("Toyota", 2020);
    std::cout << "Car 2: " << car2.brand << ", " << car2.year << "\n";

    // Using the copy constructor
    Car car3 = car2;
    std::cout << "Car 3: " << car3.brand << ", " << car3.year << "\n";

    return 0;
}
```
```
``````
Destructor
```cpp
#include <iostream>

class Car {
public:
    // Constructor
    Car() {
        std::cout << "Car created.\n";
    }
    
    // Destructor
    ~Car() {
        std::cout << "Car destroyed.\n";
    }
};

int main() {
    Car myCar; // Constructor called
    // Destructor will be called automatically when myCar goes out of scope

    return 0;
}
```
