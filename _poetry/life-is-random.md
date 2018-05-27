---
layout: post
title: Life is random
date: 2012-10-01 10:07:00
---

```java
import java.util.*;

public class Life {	
    private String brain;
    private String fate;	
    public static void main(String[] a) {
        Life I = new Life();
        I.live();
    }
	
    public void live() {
        my_destiny();
        System.out.println("I'm "+brain+" and "+fate+".");
    }
	
    private void my_destiny() {
        Random r = new Random();
        String [] fates = {"Lucky", "Unlucky"};
        String [] brains = {"Smart", "Stupid"};
        fate = fates[r.nextInt(2)];
        brain = brains[r.nextInt(2)];
    }
}
```