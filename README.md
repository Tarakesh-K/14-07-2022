1st Question

var obj1 = {"name":"Person 1","age":"5"};

var obj2 = {"age":"5","name":"Person 1"}; 

console.log(JSON.stringify(obj1) == JSON.stringify(obj2));

2nd Question

var req = new XMLHttpRequest();

req.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");

req.send();

req.onload=function(){

    var result = JSON.parse(req.response);
    
    for(i=0;i<result.length;i++){
    
      console.log(result[i].flag);
      
    }
    
}

3rd Question

var req = new XMLHttpRequest();

req.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");

req.send();

req.onload=function(){

    var result = JSON.parse(req.response);
    
    for(i=0;i<result.length;i++){
    
      console.log(result[i].name);
      
      console.log(result[i].region);
      
      console.log(result[i].subregion);
      
      console.log(result[i].population);
      
    }
    
}
