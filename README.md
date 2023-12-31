# Derivative Library

This code is a library for calculating derived functions.

## Installation

To install the library, use pip:

    pip install pyderivative==1.2

## Usage

To use the library, import the `Derivative` class from the library:

    from pyderivative.Derivative import Derivative

Then you can create an instance of the `Derivative` class by passing the function you want to differentiate as an argument:

    def func(x):
        return x**2
    derivative = Derivative(func)

## Methods

### tailor_app

Calculates the derivative of the function at the point `x0` using the Taylor method.

Usage example:

    result = derivative.tailor_app(2)

### polinom_app

Calculates the derivative of the function at the point `x0` using the polynomial method.

Usage example:

    result = derivative.polinom_app(2)

### second_derivative

Calculates the second derivative of the function at the point `x0`.

Usage example:

    result = derivative.second_derivative(2)

### threepoint_pattern(x0, second_deriv=False)

Calculates the first or second derivative of a function at the point `x0` using the three-point method.

Usage example:

    result = derivative.threepoint_pattern(2, second_deriv=True)

## Exception handling

If the function was set using a grid, the methods `tailor_app`, `polinom_app` and `threepoint_pattern` will throw an exception. If an error occurred while using the function, the methods will also throw an exception.

## License

This library is available under the MIT license.
