import Foundation

// Ex №1 (2x^2 + 3x - 4 = 0)
let Formula = "2x^2 + 3x - 4 = 0"
let a = 2
let b = 3
let c = -4
let Discriminant = (b * b) - (4 * a * c)
let One = b * -1 - Discriminant / 2 * a
let Two = b * -1 + Discriminant / 2 * a

// Ex №2 Даны катеты прямоугольного трецгольника. Найти площадь, периметр и гипотенузу треугольника.
var cathet1 = 3
var cathet2 = 4
let square = 1/2 * Double(cathet1) * Double(cathet2)
let hypotenuse = sqrt(Double(cathet1) * Double(cathet1) + Double(cathet2) * Double(cathet2))
let perimetr = Double(cathet1) + Double(cathet2) + hypotenuse

//Ex №3 Пользователь вводит сумму вклада в банк и годовой процент. Найти сумму вклада через 5 лет.
var depositAmount = 10000
let percent = 0.15
var oneYear = (Double(depositAmount) * percent) + Double(depositAmount)
var twoYear = oneYear * percent + oneYear
var threeYear = twoYear * percent + twoYear
var fourYear = threeYear * percent + threeYear
var fiveYear = fourYear * percent + fourYear
print(fiveYear)
