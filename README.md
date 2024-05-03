public class Main {  

  

  public static void main(String[] args) throws InterruptedException {  

      int rts = 0;  

  

      float x, y;  

  

      for (y = 2.5f; y > -2.0f; y -= 0.12f) {  

  

          for (x = -2.3f; x < 2.3f; x += 0.041f) {  

  

              float a = x * x + y * y - 4f;  

  

              if ((a * a * a - x * x * y * y) < -0.0f) {  

  

                  String str = "I LOVE YOU!";  

  

                  int num = rts % str.length();  

  

                  System.err.print(str.charAt(num));  

  

                  rts++;  

  

              } else {  

  

                  System.err.print(" ");  

  

              }  

  

          }  

  

          System.err.println();  

  

          Thread.sleep(100);  

  

      }  

  

  }  

  

}
