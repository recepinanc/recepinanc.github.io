# Why do we use @Override Annotation?

> “Today I learned why we use the “@Override” annotation.”

Today I wondered why we keep adding the “@Override” annotation to the top of every single method we override. 
Let’s look at the official Oracle documents:
Indicates that a method declaration is intended to override a method declaration in a supertype.
The “Override” annotation is introduced in JDK 1.5. It is used for three main reasons:
Compilers check methods that are annotated with Override to make sure the same method is declared in the supertype. If there’s a mismatch between parameter types, typo in the method name or the return type the compiler will throw a compile-time error protecting you from writing incorrect code.
It lets your IDE to warn you if the method in the parent class is changed.
It increases readability, it makes the reader of your code understand that this method overrides some other method.
Sample Usage

```
abstract class CreditCard extends CreditScoreCalculator {
    private String cardNubmer;
    abstract void pay();

    // getters & setters
}

class RecepCreditCard extends CreditCard {
    
    @Override
    public void pay() {
        System.out.println("Paid!");
    }

    private void showCreditScore() {
        calculateCreditScore();
    }
}

class CreditScoreCalculator {
    void calculateCreditScore() {
        System.out.println("Calculated: 100!");
    }
}
```

The first benefit as we’ve talked, it makes sure that the “pay(double amount)” method in OnlineCreditCard has the same method name, parameters and return type as its parent class’ CreditCard’s “pay(double amount)” method.
Secondly, if we try to change the method parameter, name or return type in CreditCard, the IDE will warn us about this change.
Image for post
The only thing different is that the “pay” method of CreditCard class accepts int instead of double and the IDE warns us about that. It says: “You said this method overrides a method, but we cannot find any method that matches with yours.”
Third, we can see that it is easier to understand that the “pay” method of OnlineCreditCard is overriding a method in the parent class — CreditCard.