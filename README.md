# First-task
Temperature conversion program 
[15/08, 12:42 pm] Sufiyan Khatik: # Temperature Conversion Program

def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def celsius_to_kelvin(c):
    return c + 273.15

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

def fahrenheit_to_kelvin(f):
    return (f - 32) * 5/9 + 273.15

def kelvin_to_celsius(k):
    return k - 273.15

def kelvin_to_fahrenheit(k):
    return (k - 273.15) * 9/5 + 32

# Main Program
temp = float(input("Enter temperature value: "))
unit = input("Enter unit (C for Celsius, F for Fahrenheit, K for Kelvin): ").strip().upper()

if unit == "C":
    f = celsius_to_fahrenheit(temp)
    k = celsius_to_kelvin(temp)
    print(f"{temp}°C is equal to {f:.2f}°F and {k:.2f}K")
elif unit == "F":
    c = fahrenheit_to_celsius(temp)
    k = fahrenheit_to_kelvin(temp)
    print(f"{temp}°F is equal to {c:.2f}°C and {k:.2f}K")
elif unit == "K":
    c = kelvin_to_celsius(temp)
    f = kelvin_to_fahrenheit(temp)
    print(f"{temp}K is equal to {c:.2f}°C and {f:.2f}°F")
else:
    print("Invalid unit entered. Please enter C, F, or K.")
[15/08, 12:42 pm] Sufiyan Khatik: Enter temperature value: 25
Enter unit (C for Celsius, F for Fahrenheit, K for Kelvin): C
25.0°C is equal to 77.00°F and 298.15K
[15/08, 12:43 pm] Sufiyan Khatik: Enter temperature value: 300
Enter unit (C for Celsius, F for Fahrenheit, K for Kelvin): K
300.0K is equal to 26.85°C and 80.33°F
