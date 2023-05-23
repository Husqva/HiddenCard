# HiddenCard
Реализуйте метод getHiddenCard(), который принимает на вход номер кредитки (всегда состоит из 16 цифр) в виде строки и возвращает его скрытую версию, которая может использоваться на сайте для отображения. Если исходная карта имела номер 2034399002125581, то скрытая версия выглядит так ****5581. Другими словами, функция заменяет первые 12 символов, на звездочки. Количество звездочек регулируется вторым необязательным параметром. Значение по умолчанию — 4.
public class App {
    // BEGIN (write your solution here)
    public static String getHiddenCard(String x) {
        x = x.substring(12, 16);
        x = "*".repeat(4) + x;
        return (x);
    }
    public static String getHiddenCard(String x, int y) {
        x = x.substring(12, 16);
        x = "*".repeat(y) + x;
        return (x);
    }
    // END
}
