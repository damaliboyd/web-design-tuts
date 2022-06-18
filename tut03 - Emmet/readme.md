# [Learn Emmet In 15 Minutes - Double Your HTML Coding Speed](https://www.youtube.com/watch?v=V8vizNQKtx0)
 Emmet is really cool.
___
- ! + enter -  creates html boilerplate
- [html element] + enter - creates starting and closing tag for said element
  - `span` => ```<span></span>>```
- [html element].[classname] + enter-  creates the html element with the class specified after the dot
  - instead of a dot a hashtag can be used to specify the id
  - if not given a html element it defaults to div
  - `.class-1`  
    ```
    <div class="class-1"></div>
    ```
  - `#id-1`  
    ```
    <div id="id-1"></div>
    ```
  - `div.class-1` 
    ```
    <div class="class-1"></div>
    ```
  - `div.class-1.class-2#id-1` 
    ```
    <div class="class-1 class-2" id="id-1"></div>
    ```
- Similar to above, attributes can be added with square brackets
  - `button[type="button]`  
    ```
    <button type="button"></button>
    ```
  - `[data-selected].active`  
    ```
    <div data-selected="" class="active"></div>
    ```
- Nesting child elements with >
  - `div.purple>span.cyan` => 
    ```
    <div class="purple"><span class="cyan"></span></div>
    ```
  - `header>nav>ul`
    ```
    <header>
        <nav>
            <ul></ul>
        </nav>
    </header>
    ```
- Mulitplication of elements with *
- {} adds text
- $ adds number based on multiplicity of item $$ gives 0 padded numbers
    - `header>ul>li*3{List Item $$}`
        ```
        <header>
            <ul>
                <li>List Item 01</li>
                <li>List Item 02</li>
                <li>List Item 03</li>
            </ul>
        </header>
        ```
- Escape from children > with carets ^
  - `header>nav>li*3{List Item $$}^^main+footer`
      ```
      <header>
          <nav>
              <li>List Item 01</li>
              <li>List Item 02</li>
              <li>List Item 03</li>
          </nav>
      </header>
      <main></main>
      <footer></footer>
      ```
- or group with parenthesis
  - `(header>nav>li*3{List Item $$})main+footer` yeilds the same as above