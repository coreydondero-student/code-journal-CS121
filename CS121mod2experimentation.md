# Guided experimentation

### ConversionFun.java. Add the following code and print the values. Record results:
 - `volume3 = PI * radiusCubed * (4 / 3);`  
    - The result is 3.14159. This is because the int values are calculated first, so 4/3 = 1.
 - `volume4 = 4 / (3 * PI) * radiusCubed;`  
    - Result is 0.42441354006516874. We are using floating point this time, but the math is incorrect (3PI is the denominator in this case, instead of just 3).

### CookieGun.java. Add the following code and print the values. Record results:
  - `cookiesPerFriend = (double) (numCookies / numFriends);`
     - The output is 2.0 because we only cast to double after the int arithmetic was done. I think the best is actually to just leave everything in int because nobody wants to split a cookie into into 2/5 of a cookie.
  - 
