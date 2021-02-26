Exercise 8.2 Why did the Dyna agent with exploration bonus, Dyna-Q+, perform
better in the first phase as well as in the second phase of the blocking and shortcut
experiments?

Na segunda fase do experiemento (após os 3000 steps) a resposta é bem clara: O Dyna-Q+ realizou explorações que o Dyna-Q provavelmente nem tentou, sendo capaz de encontrar o atalho e conseguir resultados melhores. Quanto a porque o Dyna-Q+ performou melhor mesmo antes dos 3000 passos, acredito que seja pelo controle que ele dá para a exploração, de maneira que ele mantém um registrou de quantos steps faz que ele visitou o par estado-ação, dando intervalos mais preparados do que simplesmente ir explorando.
