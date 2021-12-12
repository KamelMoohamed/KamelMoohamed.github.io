# CMP2241_Task 3 --> (const, &) uses in c++

## Table of Contents
<ul>
<li><a href="#const">Const Uses:</a></li>
    <ul>
        <li><a href="#constVar">Variables decleration</a></li>
        <li><a href="#pointers">Pointers</a></li> 
        <li><a href="#funReturn">Function Return Type</a></li>  
        <li><a href="#classData">Class Data Member</a></li>   
    </ul>
<li><a href="#andSign">& uses:</a></li>
    <ul>
        <li><a href="#and">Logical Operator (And).</a></li>
        <li><a href="#and2">Get the adress of operator.</a></li>  
    </ul>
</ul>


<a id='const'></a>
## Const Uses

<a id='constVar'></a>
### Variables decleration.
If we put the (const) keyword before the variable dataType, it will be constant and its value can't be changed later.

```
const int x = 10;
x = 5; // Error
```

<a id='pointers'></a>
### Pointers
When we use const with pointers, we can apply const to what the pointer is pointing to or we can make a pointer itself to be const.
```
// Pointer to const variable
const x = 10;
const int* w = &x;
```
```
// Constant Pointer
int const* x;
```

We can also use a const pointer to point to const variable.
```
// Constant Pointer
const int const* x;
```

<a id='funReturn'></a>
### Function Return Type
When we write a const before the function date type, the function will return a const.
```
const int returnTest(){
    return 10;
}
```

<a id='classData'></a>
### Class Data Member

```
class Test{
private:
    const int i;
public:

    Test(int x):i(x){
    }
```
In the code above (i) value will be intialized when we call the constructor and it can't be changed again.


<a id='andSign'></a>
## Const Uses

<a id='and'></a>
### Logical (And)

```
int main(){
    int x;
    cin >> x;
    if((x > 0) && (X < 10>)){
        // Any Code here
    }
    return 0;
}
```


<a id='and2'></a>
### To get the adress of an operator
```
int* x = &i;
```
