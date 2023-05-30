
pipeline
{
agent any
environment
    {
	clima = "Lluvioso"  
          
    }
	
stages
{
     
    stage("Dias de la semana")
    {
        steps
        {
            
            script
            {
                def dia = new Date().getDay()
                def map = [1: "Lunes", 2: "Martes", 3: "Miercoles", 4:"Jueves", 5:"Viernes", 6:"Sabado", 7: "Domingo"]
                println dia
                println map
				
				
				if(dia == 2 ){
				println "El usuario que inicio el trabajo es ${env.USERNAME}"
				}
				
				
				if(dia == 3 ){
				println clima
				}
				
				if(dia == 4){
			    	git branch: "main", url: "https://github.com/dahedo/CICD_jenkins.git"
				}
				
                
                
            }
        }
        
    }
}
}
