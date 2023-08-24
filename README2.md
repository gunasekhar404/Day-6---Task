*write a class to calculate the uber price.

let baseFee = .44
let cities = ["Chennai", "Hyderabad", "Banglore", ]
let uberRates = [150,200,250]
// DRY = don't REPEAT yourself
//prompts to customer
let customerName = "Wendy" //prompt("What is your name?")
let customerCity = "Providence" //prompt("What is your city?")
//after the prompts, log to console customerName and welcome
console.log("Hello", customerName+ ", welcome to the Uber Rate Program")
//function that will getRate based on customerCity
function getRate(customerCity) {
  //uberRate function that will calculate the rate based on customerCity and index
  function uberRate(customerCity, index) {
    //calculate the final rate
    let finalRate = (uberRates[index]) * baseFee
    return finalRate
  }
  //log to the console customerCity and the finalRate after calling function uberRate and passing customerCity and index as parameters
  console.log(customerCity, "rate is:", uberRate(customerCity, cities.indexOf(customerCity)))
}
//call the getRate function passing in the customerCity arugment
getRate(customerCity)
