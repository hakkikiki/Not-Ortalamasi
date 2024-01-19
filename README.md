import javax.sound.midi.Soundbank;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
      

        // Değişkenleri oluşturuyoruz
        int mat, fizik, kimya, turkce, tarih, muzik;

        Scanner test = new Scanner(System.in);
        
        // Kullanıcıdan Değer Alma işlemini yap
        System.out.print("Matematik Notu Girin : ");
        mat = test.nextInt();

        System.out.print("Fizik Notu Girin : ");
        fizik = test.nextInt();

        System.out.print("Kimya Notu Girin : ");
        kimya = test.nextInt();

        System.out.print("Turkce Notu Girin : ");
        turkce = test.nextInt();

        System.out.print("Tarih Notu Girin : ");
        tarih = test.nextInt();

        System.out.print("MÜzik Notu Girin : ");
        muzik = test.nextInt();

        int toplam = (mat + fizik + kimya + tarih + muzik);
        double sonuc = toplam / 6 ;
        System.out.println("Not Ortalamanız : " + sonuc );

        boolean kosul1 = sonuc <= 45;
        boolean kosul2 = sonuc >= 45;
        boolean karne = kosul1 || kosul2;

        String str = karne  ? "Sınıfı Geçtiniz" : "Sınıf Tekrarı";
        System.out.printf(str);




    }

}
