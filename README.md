# Mainmenu
This project consists of showing the menu of a fast food restaurant where when placed on each menu, a Hover effect is generated that changes the background color and the color of the letters to highlight the publication.

HTML:

<!DOCTYPE html>  
 <html lang="en">  
 <head>  

   <meta charset="UTF-8">  
   <meta http-equiv="X-UA-Compatible" content="IE=edge">  
   <meta name="viewport" content="width=device-width, initial-scale=1.0">  
   <title>Menu de Hamburguesa</title>  
   <link rel="stylesheet" href="./mimenucomida.css">  
 </head>  
 <body>  
 <div class="content">  
   <div class="heading">MENU PRINCIPAL</div>  
   <div class="cateogaries">  
    <a class="ctitle all" >ALL YOU CAN EAT</a>  
   </div>  
   <div class="container">  
     <div class="items">  
       <div class="img-conatiner"><img src="https://wallpapercave.com/wp/wp3151363.jpg"  
       alt="Burger" class="img"></div>   
        <div class="details">  
          <div class="title">burger</div>  
          <div class="price">$4</div>  
         </div>  
       <div class="cateogary">FAST FOOD</div>  
     </div>  
     <div class="items">  
       <div class="img-conatiner"><img src="https://static.toiimg.com/thumb/73514385.cms?imgsize=1468833&width=800&height=800"  
        alt="Burger" class="img"></div>   
        <div class="details">  
          <div class="title">burger</div>  
          <div class="price">$4</div>  
          </div>  
        <div class="cateogary">FAST FOOD</div>  
      </div>  
   </div>  
 </div>  
   <script src="./foodmenu.js"></script>  
 </body>  
 </html>  

 CSS:

 *{  
   margin: 0;  
   padding: 0;  
 }
 
 body{
	background-color: orange; 
 }
 
 .content{  
   display: flex;  
   flex-direction: column;  
   align-items: center;  
 }
 
  .heading{  
   font-size:40px;  
   font-weight: 800;  
   margin:60px auto;  
   color: blue;
 } 
 
 .cateogaries{  
   display: flex;  
   flex-wrap: wrap;  
 }  
 
 .ctitle:active{  
   background-color:rgba(255,0,0,0.9);  
 } 
 
 .cateogaries .ctitle{  
 margin:10px;  
 border:4px solid red;  
 padding: 20px 65px;  
 border-radius:12px; 
 background-color: #000000; 
 } 
 
 a{  
   text-decoration: none;  
   color:#ffffff;  
 } 
 
 .container{  
   display: flex;  
   flex-wrap: wrap;  
   width:80%;  
   justify-content:center;  
   margin: 20px;  
 } 
 
 .items{  
 width:200px;  
 height:300px;  
 display:flex;  
 border:4px solid red;  
 padding:4px;  
 border-radius: 10px;  
 margin: 20px;  
 flex-direction: column; 
 color:blue;
 }  
 
 .img{  
   width:200px;  
   height:200px;  
 }
 
 .title{  
   font-size:20px;  
 } 
 
 .cateogary{  
   text-align: center;  
   margin: 10px 0px;
     
 } 
 
 .details{  
 display: flex;  
 justify-content: space-between;  
 width:100%;  
 } 
 
 .items:hover{  
   background-color: #000000;  
   color:white;  
   transition-duration:0.7s;  
   box-shadow: 8px 8px 10px rgba(255,0,0,0.4);  
   transform:translate(-8px,-8px);  
 } 

.img-conatiner{  
   height:200px;  
   width:200px;  
   overflow: hidden;  
 } 

.cateogaries .ctitle:hover {  
   transform: translate(3px,-5px);  
   transition-duration: 0.7s;  
   box-shadow: 5px 5px 10px rgba(255,0,0,0.5);  
 }   
