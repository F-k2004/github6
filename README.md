# temperature_converter.p

def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

def main():
    print("🌡️ مبدل دما")
    print("1. سانتی‌گراد ➝ فارنهایت")
    print("2. فارنهایت ➝ سانتی‌گراد")
    
    choice = input("انتخاب کنید (1 یا 2): ")
    
    if choice == "1":
        c = float(input("دمای سانتی‌گراد: "))
        print(f"✅ {c}°C = {celsius_to_fahrenheit(c):.2f}°F")
    elif choice == "2":
        f = float(input("دمای فارنهایت: "))
        print(f"✅ {f}°F = {fahrenheit_to_celsius(f):.2f}°C")
    else:
        print("❌ انتخاب نامعتبر!")

if __name__ == "__main__":
    main()
