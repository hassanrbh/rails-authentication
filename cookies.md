# Cookies

    - Because HTTP request are stateless we need some way to create a **persistence** iacroos connections and what we needed is cookies 
![shutterstock_1295870983](https://user-images.githubusercontent.com/68386394/157446125-84fb7225-8f0c-4bf4-9f00-15ef4ab99325.png)

    - cookies are little pieces of data and are <= 4kb in size and sent down by a website to your browser
  
    - try to look at the architecture of the cookies and see what you got
    
![AHN69-Iw5AUtU1ZIRJDV3PJDrKXwuMumbdo-](https://user-images.githubusercontent.com/68386394/157446435-538818fd-c78c-44db-9717-34488b5ca303.jpg)

    - Also we have some rules here:
      - 1. The cookie is always saved in the client side
      - 2. A cookie is a giant hashmap that store that cookie
      - 3. a browser who make the permission to send the cookie to "fakeamazon.com" and it have all the power and the browser enforces all this rules
      - 4. the browser work is to enforce that only "fakeamazon.com" can see the cookies of "fakeamazon.com"
      - 5. the client side will reject a cookie if it´s more than 4kb
      - 6. each domain have a maximum of 20 cookies
      - 7. and in finale the cookie is stored in a header request
      - 8. I think you have a question in your mind and it's why this website force us to enable cookie when we enter, becauses if you not enable the cookies you will not have state and if you don't have state you cannot register or login because the browser dosen't know anything besides the mete data that will go though the header to the server side of "fakeamazon.com"
