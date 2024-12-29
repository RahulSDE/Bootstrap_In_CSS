# **BOOTSTRAP**
- Most important **Frontend Framework**.

- It is used for building responsive websites.

- **Bootstrap**, originally named as **Twitter Blueprint** was developed by **Mark Otto** and **Jacob Thorton** at twitter as a 
   framework to encourage consistency across internal tools.

- Bootstap = (Grid System + classes + components).

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


## **GRID SYSTEM**
- 
    ```
        Bootstrap Grid System
        1) BreakPoint
        2) Container
        3) Row
        4) Column
    ```

    - #### **Breakpoint**
        - Example:
        ```
            ```
            X-small                  0px   - 575px               [ col-* ]        col-lg-12   col-lg-12    col-lg-12
            small                    576px - 767px               [ col-sm-* ]     col-lg-12   col-lg-12    col-lg-12
            Medium                   768px - 991px               [ col-md-* ]     col-lg-12   col-lg-12    col-lg-12
            Large                    992px - 1192px              [ col-lg-* ]     col-lg-4    col-lg-6     col-lg-2
            Extra Large              1200px - 1399px             [ col-xl-* ]
            Extra Extra Large        1400px - Infinite           [ col-xxl-* ]
        ```

    - #### **Container:**
        - Wrapper that contain the website.
        - Websites which depends on wrapper width.
        - we put the whole content of website inside a **div tag**. This tag behaves like a container.
        - Example: Compare https://passwordsgenerator.net/ And https://www.lastpass.com/password-generator.
        - 
            ```
                <div class="container"></div>
            ```

    - #### **Row :**
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

    - #### **Column :**
        - Syntax:
            ```
                <div class="container">
                    <div class="row">
                        <div class="col-12"></div>
                    </div>
                </div>
            ```
        - **<div class="col-12"></div>** The class **col-12** combines all the 12 column into a single div.
        - Hence, we can combine these 12 columns in whichever way we want.
        - The style that we are applying on the breakpoint will remain the same for all the breakpoints above it.
        and the will change for all the breakpoints below it.
        - Ex: 
            ```
                X-small                  0px   - 575px               [ col-* ]        col-lg-12   col-lg-12    col-lg-12
                small                    576px - 767px               [ col-sm-* ]     col-lg-12   col-lg-12    col-lg-12
                Medium                   768px - 991px               [ col-md-* ]     col-lg-12   col-lg-12    col-lg-12
                Large                    992px - 1192px              [ col-lg-* ]     col-lg-4    col-lg-6     col-lg-2
                Extra Large              1200px - 1399px             [ col-xl-* ]
                Extra Extra Large        1400px - Infinite           [ col-xxl-* ]
            ```

- There are different functionalities in grid system
    - #### **Reodering:**
        - we can reoder columns at different breakpoints.
        - Syntax : 
        ```
            order-lg-2 ----> what it is saying that at large screen the order of the div will be 2.
        ```

        - Ex:
        ```
            <div class="container-fluid">
                <div class="row" style="min-height: 200px;">
                    <div class="col order-lg-2 bg-primary text-white">div1</div>
                    <div class="col order-lg-3 bg-danger text-white">div2</div>
                    <div class="col order-lg-1 bg-success text-white">div3</div>
                </div>
            </div>
        ```

    - #### **Offsetting Columns** 
        - means giving space from the left side.
        - Example:
        ```
                <div class="container-fluid">
                    <div class="row" style="min-height: 200px;">
                        <div class="col-4 offset-2 bg-primary text-white">div1</div>
                        <div class="col-4 bg-danger text-white">div2</div>
                    </div>
                </div>
        
            In the above example, offset-2 says that the div 1 will be given 2 column space from the left side.
        ```


## **CLASSES**
- There are different classes present in bootstrap which provides us the some css functionalities which we do not need to write by 
  ourself.

- For ex:
```
    <div class="bg-primary"></div> This bg-primary class gives us the background color of blue.
    <div class="text-white></div> This text-white class gives us the text color of white
```

## **COMPONENTS**
+ #### **Accordion**
+ #### **Alerts**




