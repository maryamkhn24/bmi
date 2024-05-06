#include <iomanip> 
#include <iostream> 
#include <math.h> 
using namespace std; 
  
// C++ program to illustrate 
// how to calculate BMI 
float BMI(float height, float weight) 
{ 
    float bmi = weight / pow(height, 2); 
    return bmi; 
} 
int main() 
{ 
    float height = 1.79832; 
    float weight = 70; 
    // Function call 
    float bmi = BMI(height, weight); 
    cout << "The BMI is " << setprecision(15) << bmi 
         << " so "; 
    // Conditions to find out BMI category 
    if (bmi < 18.5) 
        cout << "underweight"; 
  
    else if (bmi >= 18.5 && bmi < 24.9) 
        cout << "Healthy"; 
  
    else if (bmi >= 24.9 && bmi < 30) 
        cout << "overweight"; 
  
    else if (bmi >= 30) 
        cout << "Suffering from Obesity"; 
  
    return 0; 
}# bmi
hs
