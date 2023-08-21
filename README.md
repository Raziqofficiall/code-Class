public class Main {
    String x, y, z;

    public Main(String sizeX, String sizeY, String sizeZ) {
        x = sizeX;
        y = sizeY;
        z = sizeZ;

        try {
            String[] sizes = {"S", "M", "L"};
            System.out.println("The t-shirt size is: " + sizes[2]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("T-shirt size not available");
        }
    }

    public static void main(String[] args) {
        Main obj = new Main("S", "M", "L");
    }
}
