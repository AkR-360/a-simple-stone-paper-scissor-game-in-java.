# a-simple-stone-paer-scissor-game-in-java.
package com.company;
import java.util.Random;
import java.util.Scanner;

public class Game {
    public static void main(String[] args) {
        /*0--->Rock
        1--->Paper
         2--->Scissor
         */
        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        int comp_choice = rand.nextInt(3);
        System.out.println("0--->Rock\n1--->Paper\n2--->Scissors\n");
        System.out.println("What do you choose:\t");
        int user_choice = sc.nextInt();


        System.out.printf("You choose %d\n", user_choice);
        System.out.printf("Computer choose %d\n", comp_choice);


            if (comp_choice == user_choice) {
                System.out.println("Its a Draw");
            } else if (comp_choice == 0 && user_choice == 1) {
                System.out.println("You Won");
            } else if (comp_choice == 0 && user_choice == 2) {
                System.out.println("Computer win");
            } else if (comp_choice == 1 && user_choice == 0) {
                System.out.println("Computer Won");
            } else if (comp_choice == 1 && user_choice == 2) {
                System.out.println("You Won");
            } else if (comp_choice == 2 && user_choice == 0) {
                System.out.println("You Won");
            } else if (comp_choice == 2 && user_choice == 1) {
                System.out.println("Computer Won");
            } else {
                System.out.println("Sorry you choose wrong number to compete");
            }
        }

}
