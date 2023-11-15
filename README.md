# PolygonAreaCalculator

This repository is a solution for the [FreeCodeCamp Scientific Computing with Python - Polygon Area Calculator](https://www.freecodecamp.org/learn/scientific-computing-with-python/scientific-computing-with-python-projects/polygon-area-calculator) problem.<br>
The PolygonAreaCalculator is a Python project that provides classes for calculating the area, perimeter, and other properties of rectangles and squares.

## Class Documentation
- **Rectangle**
  - **__init__(self, width, height):** Initializes a rectangle with the given width and height.
  - **set_width(self, width):** Sets the width of the rectangle.
  - **set_height(self, height):** Sets the height of the rectangle.
  - **get_area(self):** Calculates and returns the area of the rectangle.
  - **get_perimeter(self):** Calculates and returns the perimeter of the rectangle.
  - **get_diagonal(self):** Calculates and returns the diagonal of the rectangle.
  - **get_picture(self):** Returns a string representation of the rectangle as a picture.
  - **get_amount_inside(self, shape):** Calculates and returns the number of smaller shapes that can fit inside the rectangle.
  - **__str__(self):** Returns a string representation of the rectangle.
  - 
- **Square**
  - **__init__(self, side):** Initializes a square with the given side length.
  - **set_side(self, side):** Sets the side length of the square.
  - **set_width(self, width):** Sets the width of the square (overrides the parent method).
  - **set_height(self, height):** Sets the height of the square (overrides the parent method).
  - **__str__(self):** Returns a string representation of the square.

## Usage
The project includes two main files:

- **shape_calculator.py:** Contains the Rectangle and Square classes for calculating properties of rectangles and squares.
- **main.py:** Demonstrates the usage of the classes and includes basic tests.

Run the main.py script to see the functionality in action

## Example Usage

```python
rect = shape_calculator.Rectangle(10, 5)
print(rect.get_area())
rect.set_height(3)
print(rect.get_perimeter())
print(rect)
print(rect.get_picture())

sq = shape_calculator.Square(9)
print(sq.get_area())
sq.set_side(4)
print(sq.get_diagonal())
print(sq)
print(sq.get_picture())

rect.set_height(8)
rect.set_width(16)
print(rect.get_amount_inside(sq))
```
## Dependencies
The project does not have external dependencies beyond the Python standard library.
