![FACULTY_STAFF](https://github.com/Sanjayamagar/wt-lab-assignment/blob/master/Assignment/Assignment8/Assignment8.png)

## SORTING :

  - Sorting refers to ordering data in an alphabetical, numerical order and increasing or decreasing fashion according to some linear relationship among the data items.Sorting greatly improves the efficiency of searching.

## SORTING FUNCTIONS FOR ARRAYS IN PHP : 

  1. sort() :

     - sorts arrays in ascending order

     - Example : 
       
        ```
        <?php
          $numbers = array(40, 61, 2, 22, 13);
          sort($numbers);
  
          $arrlength = count($numbers);
          for($x = 0; $x < $arrlength; $x++) {
          echo $numbers[$x];
          echo "<br>";
          }
          ?>

          Output : 

          2
          13
          22
          40
          61

        ``` 


  2. rsort() :
          
        - sorts arrays in descending order
        
        - Example :

        ```
        
        <?php
          $numbers = array(40, 61, 2, 22, 13);
          rsort($numbers);
    
          $arrlength = count($numbers);
          for($x = 0; $x < $arrlength; $x++) {
          echo $numbers[$x];
          echo "<br>";
          }
          ?>

          Output :

          61
          40
          22
          13
          2

        ```
  3. asort() :
          
        - sorts associative arrays in ascending order, according to the value.
        - Example :

        ```
 
           <?php
            $age = array("ayush"=>"54", "shankar"=>"45", "kailash"=>"41");
            asort($age);
              
            foreach($age as $x => $x_value) {
            echo "Key=" . $x . ", Value=" . $x_value;
            echo "<br>";
            }
            ?>

            Output : 
            
          Key=kailash, Value=41
          Key=shankar, Value=45
          Key=ayush, Value=54
                  
        ``` 
 
  4. ksort() :
          
        -  sorts associative arrays in ascending order, according to the key
        
        - Example :

          ```

           <?php
           $age = array("ayush"=>"23", "shankar"=>"47", "kailash"=>"41");
           ksort($age);
             
           foreach($age as $x => $x_value) {
           echo "Key=" . $x . ", Value=" . $x_value;
           echo "<br>";
           }
           ?>
           
          Output :
           
           Key=Ayush, Value=23
           Key=Kailash, Value=41
           Key=Shankar, Value=47

          ```

  5. arsort() :
          
        -  sorts associative arrays in descending order, according to the value
  
        - Example :

          ```
           
           <?php
           $age = array("ayush"=>"23", "shankar"=>"47", "kailash"=>"41");
           arsort($age);
             
           foreach($age as $x => $x_value) {
           echo "Key=" . $x . ", Value=" . $x_value;
           echo "<br>";
           }
           ?>

          
           Output :

           Key=Shankar, Value=47
           Key=Kailash, Value=41
           Key=Ayush, Value=23

          ```

  6. krsort() :
          
        - sorts associative arrays in descending order, according to the key

        - Example :

          ```
          
           <?php
           $age = array("hari"=>"23", "ram"=>"47", "om"=>"41");
           krsort($age);
             
           foreach($age as $x => $x_value) {
           echo "Key=" . $x . ", Value=" . $x_value;
           echo "<br>";
           }
           ?>
           
          Output :

           Key=ram, Value=47
           Key=om, Value=41
           Key=hari, Value=23

          ```