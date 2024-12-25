## **BOOTSTRAP**
- Most important **Frontend Framework**.

- It is used for building responsive websites.

- **Bootstrap**, originally named as **Twitter Blueprint** was developed by **Mark Otto** and **Jacob Thorton** at twitter as a 
   framework to encourage consistency across internal tools.

- Bootstap = (Grid System + classed + components).

- `Grid System` : 
    - for responsiveness.
    - Bootstrap uses **grid system** to make websites responsive.

- `Classes` : 
    - In bootstrap, there are some classes whose CSS is already written, we just need to use those classes.
    - These classes provides us some css functionality like there are separate classes to change the background color.

- `Components`:
    - Bootstrap gives us the access of some html and css components like **Button, Alert** and many more.

- Official website for documentation : https://getbootstrap.com/

- There are two ways by which we can use **Bootstrap** in our file
    - 1) CDN.
    - 2) download and attach.

    - #### **CDN**
        - CDN : content delivery network.
        - It is a server which is very fast and hence loads the bootstrap at a very fast pace.


### **GRID SYSTEM**
- 
    ```
        Bootstrap Grid System
        1) BreakPoint
        2) Container
        3) Row
        4) Column
    ```

- `Container`:
    - Wrapper that contain the website.
    - Websites which depends on wrapper width.
    - we put the whole content of website inside a **div tag**. This tag behaves like a container.
    - Example: Compare https://passwordsgenerator.net/ And https://www.lastpass.com/password-generator.
    - 
        ```
            <div class="container"></div>
        ```

- `Row` :
    - Row is a div which contain column.
    - Div with column must be in row parent. col div cannot be inside a col div.
    - When you define a div with row class, it divide that div into 12 column.
    - Syntax:
        ```
            <div class="container">
                <div class="row"></div>
            </div>
        ```
    
    - It is divided into 12 columns and this is called **Grid system**.
    - These 12 columns is called 12 Grids.

- `Column` :
    - Syntax:
        ```
            <div class="container">
                <div class="row">
                    <div class="col-12"></div>
                </div>
            </div>
    - **<div class="col-12"></div>** The class **col-12** combines all the 12 column into a single div.
    - Hence, we can combine these 12 columns in whichever way we want.
    - The style that we are applying on the breakpoint will remain the same for all the breakpoints above it.
      and the will change for all the breakpoints below it.
      - Ex: 
            ```
                <div class="container-fluid " id="red">
                    <div class="row" id="green">
                        <div class="col-lg-6 bg-primary text-white">col-6</div>
                        <div class="col-lg-4 bg-secondary text-white">col-4</div>
                        <div class="col-lg-2 bg-danger text-white">col-2</div>
                    </div>
                </div>
            ```

            ```
                X-small                       0px   - 575px               [ col-* ]          col-lg-12   col-lg-12    col-lg-12
                small                         576px - 767px               [ col-sm-* ]       col-lg-12   col-lg-12    col-lg-12
                Medium                        768px - 991px               [ col-md-* ]       col-lg-12   col-lg-12    col-lg-12
                Large                         992px - 1192px              [ col-lg-* ]       col-lg-4    col-lg-6     col-lg-2
                Extra Large                   1200px - 1399px             [ col-xl-* ]
                Extra Extra Large             1400px - Infinite           [ col-xxl-* ]



