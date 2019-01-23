---
layout: project
type: project
image: images/java.png
title: Battle Simulation Game
permalink:
# All dates must be YYYY-MM-DD format!
date: 2018-03-20
labels:
  - java
summary: A simple text-based battle simulator I created for a college course.
---

  This text-based game is intended to model the Pokemon videogames.  I created the project using Java for an 'Introduction to Computer Science' course. It allows two players to choose monsters, and command them in a head to head fight.
  
  Some classes were already provided or needed only minor adjusments.  The first pokemon object, Bulbasaur.java, was given as a template for the rest. The code for the battle simulator, PokeBattle.java, was implemented from scratch by myself; along with the player object, Trainer.java.  To make the main method as clean as possible, it was completed using a single method call.
  
  ```
  //PokeBattle.java's main method:
  
  public static void main(String[] args) {

		// creates Trainers(Players)
		Trainer p1 = new Trainer();
		Trainer p2 = new Trainer();

		System.out.println("WELCOME! TO POKEMON FIGHT CLUB!!");
		delay();
		System.out.println("Two Trainers enter!  One Trainer leaves!");
		delay();
		System.out.println("  TEST YOUR MIGHT!  POKE'FIGHT!!!!  ");
		delay();

		do {
			System.out.println("************MAIN MENU************");
			System.out.println("1:  Choose Pokemon for Trainer 1");
			System.out.println("2:  Choose Pokemon for Trainer 2");
			System.out.println("3:  Battle");
			System.out.println("4:  View Stats for Chosen Pokemon");

			choice = input.nextLine();

			switchBoard(p1, p2); //primary function of main
			
		} while (true);

	} // end of main driver
  ```
  
  The project was created by combining the use of abstract types, subclasses, methods, user input, and interfaces.  The choice to complete it with a single method, switchBoard(p1,p2), was a self driven challenge to make the code as modular as possible.  WOrking in this way helped me learn more about using method calls and parameters to keep code as succinct as possible. <a href="https://github.com/cardinalli-uh/battlesim/tree/dev">See more here!</a>

<a href="https://github.com/cardinalli-uh/battlesim/tree/dev">
<img class="ui centered rounded huge image" src="/images/ssbattlesimrepo.png">
