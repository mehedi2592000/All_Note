hi This Is All Jquery 

1=== Satrt up====
    $(document).ready(function(){
      Console.log("hellow");
    });
      -----------
    $(function(){

    });
------------------
==> select class and id or Tag
    - $("#id)                - $("ul li") ++ if you change all ul under li data
    - $(".className")        - $("h1,div,p") 
    - $("p")                 - $("li:event") only li event row change
                             - $("li:odd") onli li odd row change 
==> Mouse Event 
    - Click()               -- when you click 
    - dblclick()            -- when you give double click
    - contextmenu()         -- if you right click on the div and you want to change the div 
    - mouseenter()          -- wnen mouse enter the div then you can change
    - mouseleave()          -- out of the div 
\
==> From Submit 
    - focus()               -- when you work in 0ne input file and you want to focus it
    - blur()                -- when you work focus then move the focus to use blur
    - change()              -- if you change the select value then it work
    - select()              -- if select in the mouse any text then you change those select value
    - submit()        
==> Get Methode 
    - text()                -- show full text of the id && if you change data then use 
    - html()                -- show full html of the id $$ if you change html 
    - attr()                -- any tag value you want to use $$ add class then change anything
    - val()                 -- input type box use to see the value 
    - addClass()            -- in html you can add class Name
    - removeClass()          -- you can remove the class name
    - $('#box').css("background","pink")  -- add css
      $('#box').css({"background","pink", "color","red"})  multiple css add

==> On and Off Event
    - on                     -- when you want to use multiple even(click, mouseevent, hoaver) handel in one id 
      $("#box").on({
          "click" :function(){
              $(this).css("background","orange");
            },
            "mouseover" : function(){
               $(this).css("background", "pink")
               }
          });


  ==> Append and Prepand
      - Append()                 --  you want add new html in this div below
      - prepand()                -- you want to add new html in this div upper
      - After()                  -- same but new html show out of the div (below)
      - Before()                  -- same same (upper)
    
== > Remove and empty
      - empty()                  -- when you want to empty in div data
      - remove()                  -- when you remove the div and div data 

==> ReplaceWith and replace all
      -replacewith()             -- if you replace on div data 
      - replacewith()            
==> warp unwarp

==> show, hide, toggle , Fadeto
    - show()            ---it show the all div html
    - hide()            -- it hide all dive html
    - toggle()          -- one click hide second click show 
    - fadeto()          -- suppos anyone click then you want to blur this portion 

