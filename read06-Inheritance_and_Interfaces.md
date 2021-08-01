Real-world objects contain ___ and ___.
A software object's state is stored in ___.
A software object's behavior is exposed through ___.
Hiding internal data from the outside world, and accessing it only through publicly exposed methods is known as data ___.
A blueprint for a software object is called a ___.
Common behavior can be defined in a ___ and inherited into a ___ using the ___ keyword.
A collection of methods with no implementation is called an ___.
A namespace that organizes classes and interfaces by functionality is called a ___.
The term API stands for ___?


Answers:

1. behaviors and properties
2. a property
3. methods
4. encapsulation
5. class
6. class, subclass, "inherits" 
7. interface
8. package
9. Application Programming Interface

package com.company;
public interface Container {

    public void addItem(int amountInML);
    public void removeItem(int amountInML);

    public int getCurrentMlInContainer();

    public int getMaxMlContainerCanHold();
}

package com.company;

public class LiquidBottle implements Container {
    int maxMl;
    int currMl;

    public LiquidBottle(int MaxVolume){
        maxMl = MaxVolume;
        currMl=0;
    }

    @Override
    public void addItem(int amount){
        this.currMl= this.currMl+amount;
    }

    @Override
    public void removeItem(int amountInML) {
         this.currMl = this.currMl-amountInML;
    }

    @Override
    public int getCurrentMlInContainer() {

        return currMl;
    }

    @Override
    public int getMaxMlContainerCanHold() {
        return maxMl;
    }
}

package com.company;

public class TwoLiterBottle extends LiquidBottle {

    public TwoLiterBottle(int MaxVolume) {
        super(2000);
    }
}


