

<template>

<v-img class="image">
  <v-app id="inspire">
    <!--
    <v-content>
      <v-col>
        <div class="title mb-1"></div>
        
            <v-img
              src="https://picsum.photos/id/1027/2848/4272"
              
              height="700"
              width="100%"
              contain
              class="grey darken-4"
            ></v-img>
            
           </v-col>
           -->
   
      <v-container
       
        class="fill-height"
        fluid
      >
        <v-row
          align="top"
          justify="center"
        >
          <v-col
            cols="100"
            sm="80"
            md="30"
          >
           <v-toolbar-title>
                 
                
                  <div class="display-4">
                    <div class="font-weight-black" >
                  

                  C O S W E A L
                  
</div>
                    </div>

                </v-toolbar-title>
             <v-toolbar-title>
               


                </v-toolbar-title>
                <v-toolbar-title>
                 <div class="font-weight-black">
                  
               <h2> Enter your e-mail and password to Log in
               </h2>
</div>
                


                </v-toolbar-title>
                <div class="flex-grow-1"></div>
                <v-tooltip bottom>
                  <template v-slot:activator="{ on }">
                    
                  </template>
                  
                </v-tooltip>
                <v-tooltip right>
                  <template v-slot:activator="{ on }">
                    <v-btn 
                      icon
                      large
                      href="https://codepen.io/johnjleider/pen/pMvGQO"
                      target="_blank"
                      v-on="on"
                    >
                  
                    </v-btn>
                  </template>
                  
                </v-tooltip>
             
              
                <v-form>
                  <v-text-field
                    label="Login"
                    name="login"
                 
                    type="text"
                  ></v-text-field>

                  <v-text-field
                    id="password"
                    label="Password"
                    name="password"
                  
                    type="password"
                  ></v-text-field>
                </v-form>
                
      <p>{{ selected }}</p>
      



              <v-card-actions>

       <input class = "rember"  color =black type="checkbox"  checked v-model="selected" ><span class="rember" >&emsp; remember id/password </span>                  
                <v-low>
          
               
     
   
 

                <div class="flex-grow-1"></div>
                <v-btn class="abc" block color="primary">Login</v-btn>
              

                </v-low>
              
              
   
<a class="link" href="http://www.cosweal.com/main/main.php">
      
    <div> forget id/password? </div>
     </a>

              </v-card-actions>
             <v-row justify="space-around" class="mb-2">
      <span class="group pa-2">
      <a class="link" href="http://www.cosweal.com/main/main.php">
      
     <v-icon btn large color="black">help_outline</v-icon>
     </a>
      </span>
 </v-row>
 <div color= "black" class="font-weight-black" id=about>
               
      

     
               <h4> About COSWEAL
               </h4>

</div>



          </v-col>
        </v-row>
      </v-container>
  </v-app>
  </v-img>


</template>>


 

<script>
  export default {
    props: {
      source: String,
    },
    data: () => ({
      drawer: null,
    }),
  }
</script>
<style>
v-low {
    margin-left: 28%;
    margin-top: 2%
}
.icon{
  margin-left: 10%
}
#about{
  color: black
}
#inspire{
    background-image: url('./assets/bg1.png.png')
}
.rember
{
   margin-left: 0 ;
text-align: center;

}
#about{
  margin-left: 42%;
}
.link{
text-decoration:none;
color: #000000;
margin-left: 30%;
text-align: center;
margin-top: 3.9%
}
.link a{

color: #000000;
}
.a{

color: #000000;
}

.v-application .accent--text {
    color:black;
    caret-color: black;
}

.v-card__actions > a.link{
color:black;
}
</style>