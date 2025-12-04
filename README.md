# UKLsoal2[UKL2.java](https://github.com/user-attachments/files/23922766/UKL2.java)
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */


package com.mycompany.ukl2;
import java.util.Scanner;

/**
 *
 * @author Danielrorrrrr
 */
public class UKL2 {

    public static void main(String[] args) {
       
        Scanner scanner = new Scanner(System.in);
        
        
        int[] pecahan = {100000, 50000, 20000, 10000, 5000, 2000, 1000};
        
        System.out.print("Input: Jumlah uang dalam rupiah : ");
        int jumlahUang = scanner.nextInt();
        
        System.out.println("\nOutput:");
        
        
        for (int i = 0; i < pecahan.length; i++) {
            int jumlahLembar = jumlahUang / pecahan[i];
            if (jumlahLembar > 0) {
                System.out.println(jumlahLembar + " Lembar " + pecahan[i]);
                jumlahUang = jumlahUang % pecahan[i]; 
            }
        }
        
      
    }
}
    

