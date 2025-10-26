Project: automaton
Aothors: David J. Barnes and Michael Kölling

This project is part of the material of the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

It is discussed in chapter 7.

26.done
27. yes
28. it turns the state of the cells to 0
29. the pattern did not change, yes they are deterministic, and yes
30. for(int i = 0; i < state.length; i++) {
            int left, center, right;
            left = (i == 0) ? 0 : state[i - 1];
            center = state[i=1];
            right = (i + 1) < state.length ? state[i+1] : 0;
            nextState[i] = (left + center + right) % 2;
        }
31. We use nextState so the current row stays unchanged while calculating the next one.
    the automaton's behavior is different after changing the assignment, but im not
    sure why.
    
32. 