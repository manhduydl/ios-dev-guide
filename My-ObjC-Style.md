
Return instead of using if else

```objc
if(error) {
  //! failure code
  return;
}

//! success code
```

```objc
if(!error) {
  //! success code
} else {
  //! failure code
}
```
