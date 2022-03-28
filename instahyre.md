```

function sleep(ms) {
      return new Promise(resolve => setTimeout(resolve, ms));
   }


async function jobApply() {
for (let i = 0; i < 30; i++) {
  a = document.getElementsByClassName("application-modal-wrap")[0].children[2].children[1].children[0]
  angular.element(a).triggerHandler("click")
  await sleep(1000)
  b = document.getElementsByClassName("application-modal-wrap")[4].children[2].children[0].children[0].children[0]
  angular.element(b).triggerHandler("click")
  await sleep(2000)
}
} 

jobApply()
```
