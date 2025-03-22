#include <iostream>
using namespace std;

class Rectangle 
{
private:
    double width;
    double height;

public:
    // No-arg constructor
    Rectangle() 
	{
        width = 1;
        height = 1;
    }

    // Parameter constructor
    Rectangle(double w, double h) 
	{
        width = w;
        height = h;
    }

    // Accessor functions
    double getWidth() const 
	{
        return width;
    }

    double getHeight() const 
	{
        return height;
    }

    // Mutator functions
    void setWidth(double w) 
	{
        width = w;
    }

    void setHeight(double h) 
	{
        height = h;
    }

    // Function to calculate area
    double getArea() const 
	{
        return width * height;
    }

    // Function to calculate perimeter
    double getPerimeter() const 
	{
        return 2 * (width + height);
    }
};

int main() 
{
    // Creating two Rectangle objects
    Rectangle rect1(4, 40);
    Rectangle rect2(3.5, 35.9);

    // Display properties and calculations
    cout << "Rectangle 1:" << endl;
    cout << "Width: " << rect1.getWidth() << ", Height: " << rect1.getHeight() << endl;
    cout << "Area: " << rect1.getArea() << ", Perimeter: " << rect1.getPerimeter() << endl;

    cout << "\nRectangle 2:" << endl;
    cout << "Width: " << rect2.getWidth() << ", Height: " << rect2.getHeight() << endl;
    cout << "Area: " << rect2.getArea() << ", Perimeter: " << rect2.getPerimeter() << endl;

    return 0;
}
