# README

## 1. Overview

    * The project consists of two java files and one test file:
        * CreditCard.java
        * CreditCardProvider.java
        * CreditCardProviderTests.java
    * The CreditCard.java file consists of the structure of a credit card object. Each card object has:
        * Card Holder Name
        * Card Number
        * Limit
        * Balance
        * Whether it is a Luhn 10 valid card or not.
    * The other class that I have created for the project is the CreditCardProvider class which allows us to make manipulations to the card according the project requirements. It consists of methods to:
        * __Add__ a new card
        * __Charge__ a valid card.
        * __Credit__ a valid card.
        * Check if the card is Luhn 10 valid or not.
        * Generate the manipulated ouput.
        * Read a file that is passed either by command line arguments or by STDIN.
    * Overall the project is pretty self explanatory, I have also added JavaDoc Comments for better undertanidng.
    * I chose to create two classes and all the different actions of the project are broken down into various methods so that it is extrmely easy to expand in future if needed.

## 2.Why Java

    * I chose java as my primary language to make the project because I feel that Object Oriented Programming can be best explained in Java. I feel java is a great language to clearly put your views through.

## 3.Compile and Run CreditCardProvider

    1. Extract the CreditCardProvider.zip file in your preferred location.

    2. Open the command line in the extracted direcotry and Compile CreditCardProvider.java with
    ```shell
    javac CreditCardProvider.java
    ```

    3. Run CrediCardProvider with either:
    ```shell
    java CreditCardProvider inputFile.txt
    ```
    or
    ```shell
    java CreditCardProvider
    ```

    4. You can also run the tests provided with JUnit, to run the tests use the following commands:
    ```shell
    javac -cp .:junit-4.12.jar:hamcrest-core-1.3.jar CreditCardProviderTests.java
    ```
    ```shell
    java -cp .:junit-4.12.jar:hamcrest-core-1.3.jar org.junit.runner.JUnitCore CreditCardProviderTests
    ```