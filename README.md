
1-	Include sass into un project
•	Install nodejs && npm
•	Npm init -y
•	Npm I sass -d
•	Create folder (sass ) then create file index.scss
•	In packge.js => scripts add “start” : “sass ./sass/index.scss ./css/style.css --watch“
•	Then open temenal in project folder and type npm start
2-	Why sass is important and powerful then css ?
•	You can use variable l
By declaring variable you can use it anywhere you want in you code
Ex (
For making un variable =
$primary-color : #eee;
$secondary-color : #fefefe
Then you can use it  =
H1{Background-color : $ primary-color ; }
)
•	You can use partials
Easy way to clean your code by include other scss files not just one file for entire project  
o	If you want to add a partial you need to create un file’s  name start with (_ ) like “_default.scss”
o	To import this file in index.scss you neet to type  ( @import “default” ) without the “_ “ or “.scss”
•	You can use mixins
You can make a mixins functions to use it more than one time
o	To make a mixins func

@mixin div_style ($prop1 , $prop2 , $prop3 ) {
Height : $prop2;
Width : $prop1;
Background-color : $prop3 ;
}
o	To include it
.header {
@include div_style(200px , 400px , black )
// rest of style
}
•	You can use extend
oTo make extend
%extend-border{
Border : 1px  solid #eee;
Padding : 10px ;
Color : #3333
}
oTo include it
.nav-bar {
@extend %extend-border ;
}




by / mahmoud okily 
