Aleksandar Chanev 186046

Control Flow Graph 
[Control Flow Graph](https://github.com/aleksandarchanev/SI_2024_lab2_186046/assets/167023315/d17472f4-b938-48fe-b431-f76b2760d458)

Цикломатската комплексност:
Цикломатската комплексност на кодот е 10,  ја добив преку формулата P+1, каде P е бројот на предикатни јазли. Во овој случај бројот на предикатни јазли е 9,па цикломатската комплексност изнесува 10.

Тест случаи според критериумот Every Branch:
Item("", "4567", 150, 5.0), payment = 120
Item("Чашка", null, 50, 0.0), payment = 50
Item("Молив", "2345", 25, 2.0), payment = 30
Item("Тетратка", "6789", 75, 3.0), payment = 100
Item("Тастатура", "3456", 500, 15.0), payment = 515

Тест случаи според Multiple Condition 
T && T && T item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode().charAt(0) == '0' 
T && T && F item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode().charAt(0) != '0' 
T && F && T item.getPrice() >= 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) == '0'
T && F && F item.getPrice() >= 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) != '0'
F && T && T item.getPrice() < 300, item.getDiscount() > 0, item.getBarcode().charAt(0) == '0' 
F && T && F item.getPrice() < 300, item.getDiscount() > 0, item.getBarcode().charAt(0) != '0' 
F && F && T item.getPrice() < 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) == '0'
F && F && F item.getPrice() < 300, item.getDiscount() <= 0, item.getBarcode().charAt(0) != '0'
