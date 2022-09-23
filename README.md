# azure-resume
My resume hosted through Azure. A personal project to get more acquainted with Azure.

# first steps
- Frontend folder contains the website
- main.js contains visitor counter code (see below)

```js
window.addEventListener('DOMContentLoaded', (event) =>{
    getVisitCount();
})

const functionApi = '';

const getVisitCount = () => {
    let count = 30;
    fetch(functionApi).then(response => {
        return response.json()
    }).then(response =>{
        console.log("Website called function API.");
        count = response.count;
        document.getElementById("counter").InnerText = count;
    }).catch(function(error){
        cibsike.log(error);
    });
    return count;
}
```

