#sailaj8247
<!DOCTYPE html>
<html>
    <head>
        <link rel = "stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/css/bootstrap.min.css">
        <script>
  
            function Calculator (){
                let distance= document.getElementById("distance").value;
let hours = document.getElementById('hoursInput');
let minutes = document.getElementById('minutesInput');
let seconds = document.getElementById('secondsInput');
let time = (+hours.value) + (+minutes.value) / 60 + (+seconds.value) / 3600
                let speed = document.getElementById("speed");
                
                console.log(distance)
console.log(time)


            
                           const result  = distance/time
document.getElementById("speed").innerHTML ="Speed:"+result;
        
    }    
        </script>
        <style> 
        table td{
        padding:    20px 10px;
        font-size: 20px;
        }
        .container{
            border: 3px solid black;
            padding: 30px;
            

        }
        </style>
    </head>
    <body>
    <div class="container">
        <div class="row">
              <h1>SpeedCalculator</h1>
            
        </div>
        <div class="row">
            <table>
                <td>speed</td> 
               <td id="speed"> </td>
               <tr>
                <td> distance</td>
                <td> <input type="number " id ="distance" name =distance><span><select>
        <option value="miles">Miles</option>
        <option value="kilometres">Kilometres</option>
    </select></span></td>
                
                <tr>
              <td> time</td>
              <td><span><input type="number" placeholder="hours" id="hoursInput"><span>
                 <span><input type="number" placeholder="mins" id="minutesInput"><span>
                  <span><input type="number" placeholder="secs" id="secondsInput"><span>
               </td>
              
              
             
		
		
		

            
               </table>
           </div>
         
               <button class ="btn btn-info" onclick="Calculator()">calculateSpeed  </button>
              <button class="btn-danger"> clear </button>
                 
               </div>
		      
		      <a href='./travel.html'>travel</a>
			</div>
             
    </body>
</html>
