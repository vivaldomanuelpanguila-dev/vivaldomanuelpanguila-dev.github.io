
// VIVALDO PANGUILA
// Funcionalidades do site

// Ano automático no rodapé
document.getElementById("year").textContent =
  new Date().getFullYear();

// Botão voltar ao topo
const topButton = document.getElementById("topButton");

window.addEventListener("scroll", function () {
  if (window.scrollY > 300) {
    topButton.classList.add("show");
  } else {
    topButton.classList.remove("show");
  }
});

topButton.addEventListener("click", function () {
  window.scrollTo({
    top: 0,
    behavior: "smooth"
  });
});

// Destacar a secção atual no menu
const sections = document.querySelectorAll("main section[id]");
const navLinks = document.querySelectorAll(".navbar a");

window.addEventListener("scroll", function () {
  let current = "";

  sections.forEach(function (section) {
    const position = section.offsetTop - 150;

    if (window.scrollY >= position) {
      current = section.getAttribute("id");
    }
  });

  navLinks.forEach(function (link) {
    link.classList.remove("active");

    if (link.getAttribute("href") === "#" + current) {
      link.classList.add("active");
    }
  });
});

console.log("Vivaldo Panguila: site carregado com sucesso!");
