# PYTHON homework 06.04.2024

Create a Python program for temperature conversion between Celsius and Fahrenheit scales.
The program should prompt users to select the direction of conversion, 
accept input for the temperature value, and accurately perform the conversion (use IF and/or ELSE).
Output should be displayed with formatted strings showing both the original and converted temperatures.

```py
try:
  print("Welcome to conversion program, where we convert temperatures between Celsius and Fahrenheit.")
  choice = input("Would you like to convert from Celsius or Fahrenheit? ").capitalize()
 
  if choice == "Fahrenheit":
    fahrenheit = int(input("What is the temperature in Fahrenheit? "))
    fahrenheit_con = (fahrenheit - 32) * 5/9
    print(f"The temperature in Fahrenheit is {fahrenheit}°F, in Celsius it is {fahrenheit_con}°C.")

  elif choice == "Celsius":
    celsius = int(input("What is the temperature in Celsius? "))
    celsius_con = (celsius * 5/9) + 32
    print(f"The temperature in Celsius is {celsius}°C, in Fahrenheit it is {celsius_con}°F.")

  else:  
    print("Please write only the word Celsius or Fahrenheit!")
    
except Exception as e:
  print(f'Wrong input, exeption: {e}')
```
