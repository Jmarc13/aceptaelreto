# aceptaelreto
# p700
// Asume fichero llamado solution.java
import java.util.HashMap;
import java.util.Map;

public class p700 {

    static java.util.Scanner in;

    public static boolean casoDePrueba() {
        int numSerie = in.nextInt();

        if (numSerie == 0)
            return false;
        else {
            Map<String, Integer> series = new HashMap<String, Integer>();

            for (int i = 0; i < numSerie; i++) {
                int serieMinutes = in.nextInt();
                String nameSerie = in.nextLine();

                if(serieMinutes >= 30){
                    series.put(nameSerie, serieMinutes);
                }

                
            }
            System.out.println(series);

            return true;
         }
    } // casoDePrueba

    

    public static void main(String[] args) {
        in = new java.util.Scanner(System.in);
        while (casoDePrueba()) {
        }
    } // main

} 
