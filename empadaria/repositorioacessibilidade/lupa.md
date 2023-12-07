/* Especifica a origem da imagem, seu tamanho e texto alternativo*/

<div class="img-magnifier-container">
    <img id="imagem1" src="link" width="600" height="400" alt="Z">
</div>

<button id="toggleLupa">Ligar/Desligar Lupa</button>

<script>
  /* Especifica a imagem pelo ID e o zoom a ser realizado pela lupa: */
  MAG.magnify("imagem1", 3);
  
  const toggleButton = document.getElementById("toggleLupa");
  const glass = document.querySelector(".img-magnifier-glass");
  
  toggleButton.addEventListener("click", () => {
    if (glass.style.display === "none") {
      glass.style.display = "block";
    } else {
      glass.style.display = "none";
    }
  });
</script>
