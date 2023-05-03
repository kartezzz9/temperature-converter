def celsius_to_fahrenheit(celsius):
    return (celsius * 9 / 5) + 32


def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5 / 9


def main():
    choice = input("Введите 'C' для конвертации из Цельсия в Фаренгейт или 'F' для конвертации из Фаренгейта в Цельсий: ")
    
    if choice.upper() == 'C':
        celsius = float(input("Введите температуру в градусах Цельсия: "))
        fahrenheit = celsius_to_fahrenheit(celsius)
        print(f"{celsius} градусов Цельсия = {fahrenheit} градусов Фаренгейта")
    elif choice.upper() == 'F':
        fahrenheit = float(input("Введите температуру в градусах Фаренгейта: "))
        celsius = fahrenheit_to_celsius(fahrenheit)
        print(f"{fahrenheit} градусов Фаренгейта = {celsius} градусов Цельсия")
    else:
        print("Некорректный выбор. Пожалуйста, попробуйте снова.")
        
if __name__ == "__main__":
    main()
