**Отчёт о тестировании приложения Precision**

**Краткое описание**
Было проведено функцинальное тестирование кода функции сложениявещественный тип данных с выведением результата в консоль

**Результаты:**

1. 100% fail
2. https://github.com/AnastasiiaGanieva/Precision/issues/1

**Рекомендации**
Добавить 0.0000000000000001 в выражение к double totalBonus:

public class Main {
    
    public static void main(String[] args) {
        double regularBonus = 0.3;
        double specialBonus = 0.6;
        double totalBonus = regularBonus + specialBonus + 0.0000000000000001;
        System.out.println(totalBonus);
    }
}
