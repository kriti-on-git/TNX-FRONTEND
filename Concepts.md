1. Node.js kya hai? Browser ke bina JS kaise chalta hai?
ye ek runtime env hai, jo javascript ko browser k bina/ bahar run krne mei needed hota hai.
browser ka v8 engine computer par available karaata hai, jisse js bdhia terminal se chlaya ja ske yay

2. npm kya karta hai?  npm install  aur  npm run dev  me fark?
npm hota hai node packager manager, ye libraries ko manage krta hai jaise react, wgrh.
npm install libraries aur dependencies install karta hai (node modules k form mei), jo ki package.json ki dependencies hoti hain, lekin npm run dev, dev server ko start karta hai jisse app app localhost pe chl sake

3.  node_modules  GitHub pe push kyun nahi karte? Delete ho jaye toh kya karoge?
node_modules ka size bahot zyda hota h cuz it includes tamaam libraries brother, plus package.json jo ki proj ka id card hai, usse wapis se bnaya jaa skta hai toh kyu faaltu mei push krna. 
.gitignore mei daalo, mentos zindagi.
aur glti se delete ho jae toh hehe npm install chlao fir se

4.  index.html  me sirf ek  <div id="root">  kyun hai?
react uss khali div ke andar sara js ui inject krta hai jisse html m manually na likhna pde sb

5. Component kya hota hai? Naam Capital letter se kyun shuru hota hai?
ui jo h, chhote chhote blocks se milke bnta hai, jise hm component kehte hain
aur dekha jaye technically, toh component ek reusable function hota hai jo ki jsx yaani ui return krta hai.
capital letter se isliye hota h shuru component ka jisse react smjh jaaye ki ye toh hmara baccha hai (react component, eg: Profile), padosi ka nahi (html tag, eg: div)


6.  main.jsx  aur  App.jsx  me kya difference hai?
main.jsx kya krta h ki, jo root of proj ko react se attach krta h jisse pp render ho ske, 
aur app.jsx mei root component ka pura ui likha jata hai
main.jsx chalayega, app.jsx dikhayega

