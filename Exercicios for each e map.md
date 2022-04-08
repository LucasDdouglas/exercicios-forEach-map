#                        For Each e Map



### Desafio 01

let students = [

  {name: "Pedro", age: 22},

  {name: "Matheus", age: 22},

  {name: "Lucas", age: 22},

  {name: "Djavan", age: 24},

  {name: "Marcos", age: 26}

]



let allstutents = 0

students.forEach( (*students*, *index*) => {

  allstutents +=  *students*.age

});



let AverageAge = allstutents / students.length



console.log(`A média da idade dos alunos é de ${AverageAge.toFixed()}`) 



### Resultado



A média da idade dos alunos é de 23



##                                             Map



### Desafio 02



let List = [

  { name: "Pedro", vip: true },

  { name: "Matheus", vip: true },

  { name: "Lucas", vip: false },

  { name: "Djavan", vip: true },

  { name: "Marcos", vip: false }

]



let Vips = List.map((*Client*) => {

  let NewList = {

​    name: *Client*.name,

​    vip: *Client*.vip,

​    sector: *Client*.vip ? "Black" : "Green"

  }

  return NewList

})

console.log(Vips)



### Resultado

[

  { name: 'Pedro', vip: true, sector: 'Black' },

  { name: 'Matheus', vip: true, sector: 'Black' },

  { name: 'Lucas', vip: false, sector: 'Green' },

  { name: 'Djavan', vip: true, sector: 'Black' },

  { name: 'Marcos', vip: false, sector: 'Green' }

 ]



### Desafio 03



let Students = [

  { name: "Pedro", testgrade: 7 },

  { name: "Matheus", testgrade: 3 },

  { name: "Lucas", testgrade: 5 },

  { name: "Djavan", testgrade: 10 },

  { name: "Marcos", testgrade: 0 }

]



let TestResult = Students.map((*result*) => {

  let allresult = {

​    Name: *result*.name,

​    Testresult: *result*.testgrade >= 7 ? "Approved" : "Disapproved"  }

 

 return allresult

})

console.log(TestResult)



### Resultado



[

  { Name: 'Pedro', Testresult: 'Approved' },

  { Name: 'Matheus', Testresult: 'Disapproved' },

  { Name: 'Lucas', Testresult: 'Disapproved' },

  { Name: 'Djavan', Testresult: 'Approved' },

  { Name: 'Marcos', Testresult: 'Disapproved' }

 ]