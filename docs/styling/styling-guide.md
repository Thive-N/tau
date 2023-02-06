Declaring once

```c
#ifndef
#endif

// over

#pragma once
```

Indentation

```c
int example(int x, int y)
{
    int sum = 0;
    if (x >= y) {return sum};
    for (int x; x < y; x++){
        sum = sum + 1;
    }
    return sum;

}

// over

int example(int x, int y)
{
    int sum = 0;
    if (x < y){
        for (int x; x < y; x++){
            sum = sum + 1;
        }
    } else {
        sum = 0;
    }
}
```

Single line statements in an if statement

```c
int example(int x) {
    if (x == 0) return 0;
}

// over

int example(int x) {
    if (x == 0) {return 0;}
}
```

```c
int example(int x) {
    if (x == 0) {return 0}
    else { return x; }
}

// over

int example(int x) {
    if (x == 0) return 0;
    else return x;
}
```
