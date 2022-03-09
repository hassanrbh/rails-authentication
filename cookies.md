# Cookies

    - Because HTTP request are stateless we need some way to create a **persistence** iacroos connections and what we needed is cookies 
  ![alt text]("https://www.elegantthemes.com/blog/wp-content/uploads/2020/10/shutterstock_1295870983.png")

    - cookies are little pieces of data and are <= 4kb in size and sent down by a website to your browser
  
    - try to look at the architecture of the cookies and see what you got
     
  ![alt text]("https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.semanticscholar.org%2Fpaper%2FHTTP-Session-Management%253A-Architecture-and-Cookies-Ayadi-Serhrouchni%2Fb95d17add8780a8e126e788c61227b3a32fa5dd5&psig=AOvVaw1s4BUXIMhy8V8IrrnMUGRY&ust=1646916138676000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCKD92O2GufYCFQAAAAAdAAAAABAD")

    - Also we have some rules here:
      - 1. The cookie is always saved in the client side
      - 2. A cookie is a giant hashmap that store that cookie
      - 3. a browser who make the permission to send the cookie to "fakeamazon.com" and it have all the power and the browser enforces all this rules
      - 4. the browser work is to enforce that only "fakeamazon.com" can see the cookies of "fakeamazon.com"
      - 5. the client side will reject a cookie if it´s more than 4kb
      - 6. each domain have a maximum of 20 cookies
      - 7. and in finale the cookie is stored in a header request
      - 8. I think you have a question in your mind and it's why this website force us to enable cookie when we enter, becauses if you not enable the cookies you will not have state and if you don't have state you cannot register or login because the browser dosen't know anything besides the mete data that will go though the header to the server side of "fakeamazon.com"