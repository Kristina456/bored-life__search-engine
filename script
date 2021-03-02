const jsForma = document.querySelector(".js-forma");
const jsDiv = document.querySelector(".js-div");

jsForma.addEventListener("submit", function (event) {
  event.preventDefault();

  deliteElement();

  fetch("https://www.boredapi.com/api/activity")
    .then((submit) => submit.json())
    .then((json) => makeNewDiv(json.activity))
    .catch((error) => console.error(error));
});

function makeNewDiv(input) {
  const div = document.createElement("div");
  div.innerHTML = `<div> ${input} </div>`;
  jsDiv.appendChild(div);
}

function deliteElement() {
  jsDiv.innerHTML = "";
}
