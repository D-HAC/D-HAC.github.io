---
layout: page
title: Degrees
permalink: /puzzle/degrees
hide: true
solutions: week1_degrees
week: 1
---

Degrees come in two main varieties in math and science. You have
degrees of a circle, and degrees of temperature (Celsius, Fahrenheit).
This week we'd like to look at both of them.

## Functions to Add to Your Code Library

### Angle Conversions

#### Degrees → Radians

```c
float degrees_to_radians(float degrees)
```

This function takes a value in degrees and converts it
to radians.

Examples:

```python
degrees_to_radians(180.0) #=> 3.1416
degrees_to_radians(45.0) #=> 0.7854
```

#### Radians → Degrees

```c
float radians_to_degrees(float radians)
```

This function takes a value in radians and converts it to
degrees.

Examples:

```python
radians_to_degrees(math.pi) #=> 180.0
radians_to_degrees(1.0) #=> 57.2958
```

### Temperature Conversions

#### Fahrenheit → Celsius

```c
float fahrenheit_to_celsius(float fahrenheit)
```

This function takes a value in °F and converts to °C.

Examples:

```python
fahrenheit_to_celsius(212.0) #=> 100.0
fahrenheit_to_celsius(32.0) #=> 0.0
```

#### Celsius → Fahrenheit

```c
float celsius_to_fahrenheit(float fahrenheit)
```

This function takes a value in °C and converts to °F.

Examples:

```python
celsius_to_fahrenheit(50.0) #=> 112.0
celsius_to_fahrenheit(100.0) #=> 212.0
```

#### Celsius → Kelvin

```c
float celsius_to_kelvin(float celsius)
```

You guessed it, this converts °C → K

Examples:

```python
celsius_to_kelvin(0.0) #=> 273.15
celsius_to_kelvin(-273.15) #=> 0.0
```

#### Kelvin → Celsius

```c
float kelvin_to_celsius(float kelvins)
```

Yup, this converts K → °C

Examples:

```python
kelvin_to_celsius(0.0) #=> -273.15
kelvin_to_celsius(273.15) #=> 0.0
```

### Notes

* Answers may differ slightly than the expected output
* Instead of having conversion methods from Fahrenheit to Kelvin,
just convert  
Fahrenheit → Celsius → Kelvin like so:

```python
celsius_to_kelvin(fahrenheit_to_celsius(32.0)) #=> 273.15
```

## Puzzle

Today's puzzle is to create a small program to convert between different units
of angle or temperature. See the below link:

[/r/dailyprogrammer: Getting a degree](https://www.reddit.com/r/dailyprogrammer/comments/4q35ip/20160627_challenge_273_easy_getting_a_degree/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these
project ideas! Feel free to make up your own project idea, but try to involve
this week's theme of unit conversions.

* Make a more robust unit converter program
    * Add other types of units to convert (distance, volume, time, etc.)
    * Maybe make it into a web page. This might be a good way to learn the
        basics of JQuery or AngularJS
    * Maybe make it into a mobile app
* Make a unit converting quiz. Make the user try to guess the result of
    a unit conversion. Use the functions we made to check the user's answer.
* If you know how to make a web server, try making a web API that converts
    units.
