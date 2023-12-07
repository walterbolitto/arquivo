/* Navegação de passagens por meio de teclado, adicionar à passagem */

(set: $key = "")
(input-box:2bind $key,"=XX=")
  (live: 1s)[(if: $key is "a")[(go-to: "passagem1")]]
  (live: 1s)[(if: $key is "s")[(go-to: "passagem2")]]
  (live: 1s)[(if: $key is "d")[(go-to: "passagem3")]]
  (live: 1s)[(if: $key is "w")[(go-to: "passagem4")]]
  (live: 1.1s)[(set: $key = "")]
