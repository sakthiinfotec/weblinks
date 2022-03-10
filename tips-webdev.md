
##### HTML
```html
<a href="tel:+1-123-456-7890">1-123-456-7890</a>
<a href="sms:+1-123-456-7890">New SMS Message</a>
<a href="mailto:friend@fb.com?subject=Hai">E-mail to Friend</a>
<a href="https://wa.me/?text=Hello">WhatsApp</a>
<p contenteditabl=true>This content is editable</p>
Credits: https://twitter.com/csaba_kissi/status/1493852940200726534?s=20&t=A3d-qYSHfyatT94emvHSzg

<!-- Edit content of a page -->
<body contenteditable> </body>
````

##### JavaScript
```javascript
/* Detect Dark Mode Preference with JavaScript */
const prefersDarkMode = window.matchMedia("(prefers-color-scheme:dark)").matches

/* Edit your live webside in Google Chrome while making Design Mode: ON */
document.designMode = 'on'

/* Computed Style */
const htmlEl = document.getElementsByTagName('body')[0]
const computedStyle = window.getComputedStyle(htmlEl)
console.log(computedStyle['backgroundColor']);  // rgb(13, 17, 23)
console.log(computedStyle['font-size'])         // 14px
console.log(computedStyle['font-family'])       // -apple-system, "system-ui", "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji"

/* Fast and easy way to create a unique ID in JavaScript */
export const uid = () => {
  const fromDate = Date.now().toString(36);
  const fromRnd = Math.random().toString(36).substr(2);
  return `${fromDate}${fromRnd}`
}

/* Display objects in a table view */
const items = [
  {id: 1, name: 'Apple'},
  {id: 2, name: 'Banana'},
  {id: 3, name: 'Carrot'},
]
console.table(items);

/* ---- Customize console log - start ---- */
const origLogFunc = console.log
console.log = (msg, err) => {
    origLogFunc.call(console, `${new Date().toGMTString()} - ${msg}`, err)
}
console.log("Hello JavaScript", new Error("Test error message"));   // Thu, 10 Mar 2022 15:24:57 GMT - Error: Test error message

// Restore back the console log
console.log = origLogFunc
/* ---- Customize console log - end ---- */

/* Prevent the user pasting text in the input box */
inputEl.addEventListener('paste', function(e){
  e.preventDefault()
})

/* Array destructure */
const fruits = ['Apple', 'Banana', 'Orange', 'Mango'];
let {0: apple, 3: mango} = fruits;
console.log(`0 => ${apple} & 3 => ${mango}`);   // 0 => Apple & 3 => Mango

```

##### Web Development
Domain: [@Namecheap](https://twitter.com/Namecheap)  
Hosting: [@vercel](https://twitter.com/vercel)  
Backend: [@Firebase](https://twitter.com/Firebase)  
Frontend Builder: [@webflow](https://twitter.com/webflow)  
Onboarding: [@intercom](https://twitter.com/intercom)  
Logo: [@logologydesign](https://twitter.com/logologydesign)  
Design: [@canva](https://twitter.com/canva)   
Copywriting: [@canva](https://twitter.com/copy_ai)   
Analytics: [@canva](https://twitter.com/PlausibleHQ)   
Email Marketing: [@canva](https://twitter.com/Mailchimp)   


##### Free Illustration Sites
```
🔹blush.design
🔹drawkit.io
🔹humaaans.com
🔹icons8.com
🔹iconscout.com
🔹illustrations.co
🔹iradesign.io
🔹isometric.online
🔹manypixels.co
🔹openpeeps.com
🔹pixeltrue.com
🔹storyset.com
🔹undraw.co
```


##### Copyright Free Images
```
1. Unsplash
2. Pexels
3. Drawkit
4. Undraw
5. Freeimages
```
Credits: [Rohith Thalla](https://twitter.com/_rohiththalla_/status/1493191519871795200)  

##### Twitter Bots
- `@pikaso_me screenshot this`
- `@SaveToNotion #thread | @SaveToNotion #Tweet`
