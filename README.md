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
